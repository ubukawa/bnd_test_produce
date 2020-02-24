task :default do
  sh "hjson -j style.hjson > style.json"
  sh "gl-style-validate style.json"
  sh "browserify -o bundle.js -t [ babelify --presets [ @babel/preset-env ] ] app.js"
end

task :tiles do
  sh "node index.js"
end

task :budo do
  sh "budo --open"
end
