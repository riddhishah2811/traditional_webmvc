# traditional_webmvc
Gives the basic understanding of why we go for Spring boot? How the traditional WebMvc worked.

## Traditional MVC Architecture
![traditional_mvc_img drawio](https://github.com/riddhishah2811/traditional_webmvc/assets/59967480/f3e12322-fcfe-4aab-b595-c51022e099cd)

## Understanding
### Dispatcher Servlet Initialization
* DispaterServlet is instantiated and initialized by the Server like Tomcat
* As part of the DispaterServlet Initialization, it loaded the appconfigurations class
* on top of appconfigurations class, we have given the Compoent scan and hence all the classes in the Component scan package were also loaded as spring beans
* InterviewResolver also loaded as a spring bean into the application context.
* RequestMappingHandler is created and registered the all the request RequestMappings because of @controller annotation
* finally Initialization is completed

### Steps we performed to create traditional mvc.
Step-1: we have identified the spring WebMvc Dependencies with the valid versions \
Step-2: We have written the Controller Class \
Step-3: we have written the view page i.e. home. jsp \
Step-4: we have written the DispaterServlet Configurations \
Step-5: We have written the AppConfigurations and enabled: \
a. webmvc configurations \
b. Component scanning \
c. Created th InternalResourceViewResolver and configured it as Spring Bean \
Step-6: we have taken an external tomcat server support and deployed the application 



