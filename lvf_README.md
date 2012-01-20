
**setup commands
 
git clone https://github.com/applieddataconsultants/Leaflet
cd Leaflet
git remote add upstream https://github.com/CloudMade/Leaflet.git
git remote add dtsagile https://github.com/dtsagile/Leaflet.git
git fetch dtsagile
git merge dtsagile/master 
#fixed conflicts
git push origin master

** build dist
sudo npm install -g jake
npm install jshint
npm install uglify-js
jake 
# errors in AGS layers from dtsagile
# cleaned up some. commented bad files out in /build/deps.js
# set jshint "bitwise": false
