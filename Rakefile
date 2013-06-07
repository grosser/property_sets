require 'bundler/setup'
require 'bundler/gem_tasks'
require 'appraisal'

require 'rake/testtask'
Rake::TestTask.new do |test|
  test.libs << 'lib'
  test.pattern = 'test/**/test_*.rb'
  test.verbose = true
end

task :default do
  sh "rake appraisal:install && rake appraisal test"
end
