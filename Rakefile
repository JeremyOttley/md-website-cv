require 'rake'

#=> rake index.html 
#=> rake index.pdf

desc "Convert index.md to index.html"
file "index.html" => ["index.md"] do |t|
	sh "pandoc index.md -s -c style.css --toc -o index.html"
end

desc "Convert index.md to index.pdf"
file "index.pdf" => ["index.md"] do |t|
	sh "pandoc index.md --template=template.tex --pdf-engine=xelatex -o index.pdf"
end
