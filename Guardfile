#LIVERELOAD

require 'cssmin'
require 'jsmin'

guard 'livereload' do

    ignore %r{^default/public/tmp/.+\.(min.css|css|min.js|js)}
    ignore %r{^default/public/bower_components/.+\.(min.css|css|min.js|js)}
    ignore %r{^default/public/css/.+\.(min.css)}
    ignore %r{^default/public/javascript/.+\.(min.js)}

    watch(%r{default/app/views/.+.(phtml)$})
    watch(%r{default/public/.+\.(css|js|html|php|phtml)})
    
    #CSS
    watch(%r[default/public/css/(.+)]) do |m|
        output_css = m[0].sub( ".css", ".min.css" )
        File.write("#{ output_css }", CSSMin.minify(File.read(m[0])))
    end

    #JS
    watch(%r[default/public/javascript/(.+)]) do |m|
        output_js   = m[0].sub( ".js", ".min.js" )
        File.write("#{ output_js }", JSMin.minify(File.read(m[0])))
    end

end