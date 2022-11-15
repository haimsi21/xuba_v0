library(golem)
library(shinyanimate)
library(shinycssloaders)
library(shiny)
library(bslib)


# La interfaz de usuario se define con ui:
ui <- fluidPage(
  
  
  
  # Application title
  #favicon(ico = "www/favi.png"),
  titlePanel(windowTitle = "Xuba  Consultoría",
             title = ""),
  
  navbarPage(
    img(src = 'mini.png', height = '30px'),
    collapsible = TRUE,
    fluid = TRUE,
    tabPanel(
      "Inicio",
      
      mainPanel(
        width = 12,
        br(), br(),
        withAnim(),
        div( id = "shinyLogo", tags$img(src= "backlogo3.png"), align="center", height = '1500px'),
        
        br(), br(),br(), br(),
        h1("está", align = "center"),
        hr(),
        h2("de vuelta", align = "center"),
        hr(),
        h2("Aquí:", align = "center"),
        hr(),
        h2(":)", align = "center"),
        br()
      )
      
    ),
    
    tabPanel("Consultoría" ,
             
             p("Equipo experto en economía, urbanismo, cartografía, finanzas, programación y diseño.|  
Uso y explotación de múltiples fuentes de información del Sistema de Cuentas Nacionales, así como las encuestas y registros administrativos del sector de interés. | 
Desempeño profesional con criterios internacionales datos, análisis e investigación.| 
Ciencia de datos: manipulación y programación para generar reportes y tomar decisiones.
"), br()),
    tabPanel("Quiénes somos"),
    
    tabPanel("Contacto"),
  )
)


#Server----


# el back-end o servidor procesa el trabajo que se muestra en ui

server <- function(input, output, session) {
 
  
  observe(addHoverAnim(session, 'shinyLogo', 'pulse'))
}
  
  

# Run the application
shinyApp(ui = ui, server = server)
