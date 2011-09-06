require 'rubygems'
require 'rake'

begin
  require 'jeweler'
  Jeweler::Tasks.new do |gem|
    gem.name = "marc2solr"
    gem.summary = %Q{MARC2Solr: Get MARC into Solr via JRuby}
    gem.description = %Q{Given a file of MARC records, send them to Sorl for indexing based on a set of MARCSpecs}
    gem.email = "bill@dueber.com"
    gem.homepage = "http://github.com/billdueber/marc2solr"
    gem.authors = ["BillDueber"]
    
    gem.add_dependency 'marc4j4r', '>= 1.3.0'
    gem.add_dependency 'jruby_streaming_update_solr_server', '>=0.5.2'
    gem.add_dependency 'marcspec', '>= 1.6.6'
    gem.add_dependency 'jruby_threach'
    gem.add_dependency 'jlogger', '>=0.0.4'
    gem.add_dependency 'library_stdnums', '>=0.2.0'
    gem.add_dependency 'trollop'
    
    gem.add_development_dependency "rspec", ">= 1.2.9"
    gem.add_development_dependency "yard", ">= 0"

    gem.bindir = 'bin'
    
  end
  Jeweler::GemcutterTasks.new
rescue LoadError
  puts "Jeweler (or a dependency) not available. Install it with: gem install jeweler"
end

# require 'spec/rake/spectask'
# Spec::Rake::SpecTask.new(:spec) do |spec|
#   spec.libs << 'lib' << 'spec'
#   spec.spec_files = FileList['spec/**/*_spec.rb']
# end
# 
# Spec::Rake::SpecTask.new(:rcov) do |spec|
#   spec.libs << 'lib' << 'spec'
#   spec.pattern = 'spec/**/*_spec.rb'
#   spec.rcov = true
# end
# 
# task :spec => :check_dependencies
# 
# task :default => :spec

begin
  require 'yard'
  YARD::Rake::YardocTask.new
rescue LoadError
  task :yardoc do
    abort "YARD is not available. In order to run yardoc, you must: sudo gem install yard"
  end
end
