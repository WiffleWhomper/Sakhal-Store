# Sakhal-Store
Custom Structure JSON Files For Console and PC Instructions ONLY WORKS ON DAYZ 1.26 AND LATER!!! NOT EARLIER VERSIONS!!!

Store created for players on my xbox community server. Inside of an otherwise empty airplane hangar; you now have shelving full of supplies to make it easier to battle the post-apocalyptic archipelago of Sakhal.

Limited testing was conducted on Xbox Series S using DayZ Version 1.26 as of March 2025.

Created by @WiffleWhomper. For bug reports or issues, please email c.lindberg823@gmail.com with relevant screenshots.

If you'd like to edit any file, simply load the .DZE file into the DayZ Editor.

TERMS OF USE THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

Using these modded JSON files and instructions could break the functioning of your DAYZ server, requiring a reinstall that would wipe all player progress.

Using these modded files necessitates increased regular restarts to prevent server crashing.

It is strongly recommended that you thoroughly test your server after applying these files to ensure the proper functioning of your server.

I always recommend validating your files at:

https://www.xmlvalidation.com/

https://jsonlint.com/





Instructions:

Stop Your Server Ensure your server is offline before proceeding.

Ensure you activate cfggameplay.json 

 Nitrado Console Servers:
  -   Settings >> General >> tick Enable cfggameplay.json. 

 For PC Servers, add the following line to your serverDZ.cfg:

 -  enableCfgGameplayFile = 1; 

   (Note: For some PC servers, including Nitrado, the serverDZ.cfg may be hidden. To access it, enable "Expert Mode" in your settings, then navigate to "Expert Settings" to find serverDZ.cfg. Remember to stop the server before making changes.)

 Upload your file:

  Tools >> File Browser >> dayzxb_missions >> dayzOffline.Sakhal >> custom >> "Upload File" 
 
   (If a custom folder doesn't exist, create one.)

Call to the custom file using the cfggameplay.json  

 Tools >> File Browser >> dayzxb_missions >> dayzOffline.Sakhal >> cfggameplay.json

          "WorldsData":
        	{
        		"lightingConfig": 2,
        		"objectSpawnersArr": [],
        		"environmentMinTemps": [-6.5, -9.5, -6.5, -9.5, 2, 6, 9, 10, 6, 1, -5, -10],
        		"environmentMaxTemps": [-3, -5, -3, -5, 9, 14, 16, 17, 14, 8, 1, -3],
        		"wetnessWeightModifiers": [1.0, 1.0, 1.33, 1.66, 2.0],
        		"playerRestrictedAreaFiles": ["pra/warheadstorage.json"]
        	},

Edit the objectSpawnerArr to look like this:

"objectSpawnersArr": ["custom/sakhalstore.json"]

 If you're already calling other custom JSONs to spawn items or buildings, separate them with commas:

"objectSpawnersArr": ["custom/sakhalstore.json", "custom/anotherfile.json", "custom/differentfile.json"] 

   
   EXAMPLE OF YOUR NEW FILE         

         
          "WorldsData":
        	{
        		"lightingConfig": 2,
        		"objectSpawnersArr": ["custom/sakhalstore.json", "custom/anotherfile.json", "custom/differentfile.json"],
        		"environmentMinTemps": [-6.5, -9.5, -6.5, -9.5, 2, 6, 9, 10, 6, 1, -5, -10],
        		"environmentMaxTemps": [-3, -5, -3, -5, 9, 14, 16, 17, 14, 8, 1, -3],
        		"wetnessWeightModifiers": [1.0, 1.0, 1.33, 1.66, 2.0],
        		"playerRestrictedAreaFiles": ["pra/warheadstorage.json"]
        	},

     

SAVE YOUR FILE

restart your server and the new store will spawn with all items ready for use.

Thanks, and happy gaming! Created by @WiffleWhomper For support or inquiries: WiffleWorkShop@gmail.com
