require 'rubygems'
require 'rake/packagetask'
require 'rake/gempackagetask'

spec = Gem::Specification.new do |s| 
  s.name = "wkhtmltopdf-binary"
  s.version = "0.9.9"
  s.author = "Research Information Systems, The University of Iowa"
  s.email = "vpr-ris-developers@iowa.uiowa.edu,mcollas@aconex.com"
  s.platform = Gem::Platform::RUBY
  s.summary = "Provides binaries for WKHTMLTOPDF project in an easily accessible package."
  s.files = FileList["{bin,libexec,lib}/*"].to_a
  s.has_rdoc = false
  s.executables << "wkhtmltopdf"
  s.require_path = '.'
end

Rake::GemPackageTask.new(spec) do |pkg|
  pkg.need_tar = true
end
