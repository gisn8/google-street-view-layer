## <img src="icon.png" style="width:24px;height:24px;"> Google Street View Layer

A QGIS processing plugin that uses your road layer, and creates a new or joinable layer or table with the most recent 
Google Street View capture data.  
  
**Google API Key required!**

For best results, if not already, it is advised your road layer be broken down at least block by block. If necessary, 
the Vector overlay > Split with lines QGIS processing tool should work for this by selecting your initial road layer for
both inputs. Be sure you QA/QC and get familiar with the result before proceeding.

### TESTING MODE:

Among the initial variables set in google_street_view_layer_algorithm.py is "testing = 0".

Testing mode set to 0 will let the plugin operate as expected. 

Testing mode set to 1 will:
- Print to the console the process functions being accessed, and important variable values along the way.
- Unless a valid API key is entered, will assume anything entered under 39 characters is initially valid; if
key given is invalid, the status on the calls will always be REQUEST DENIED. A valid key may be used during
testing and will make legitimate API calls that could result in charges from Google; a very small sample layer is
strongly suggested; USE WITH CAUTION!

### KNOWN BUGS

There are a few known issues that doesn't hinder the process, but do have minor impacts on the user's overall 
experience. Please review the Issues page at https://github.com/gisn8/google-street-view-layer/issues.
