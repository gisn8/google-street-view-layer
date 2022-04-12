### <img src="icon.png" style="width:24px;height:24px;"> Google Street View Layer

A QGIS processing plugin that uses your road layer, and creates a new or joinable layer or table with the most recent Google Street View capture data.  
  
**Google API Key required!**

For testing:

Among the initial variables set in google_street_view_layer_algorithm.py is "testing = 0".

Testing mode set to 0 will let the plugin operate as expected. 

Testing mode set to 1 will:
- Print to the console the process functions being accessed, and important variable values along the way.
- Unless a valid API key is entered, will assume anything entered under 39 characters is initially valid; if
key given is invalid, the status on the calls will always be REQUEST DENIED. A valid key may be used during
testing and will make legitimate API calls that could result in charges from Google; a very small sample layer is
strongly suggested; USE WITH CAUTION!
