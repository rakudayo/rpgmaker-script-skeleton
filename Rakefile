require 'bundler/setup'

Bundler.require(:default, :development)

task default: %w[spec]

desc 'Load the environment'
task :environment do
  require_relative 'environment'
end

desc "Start a console with app environment loaded"
task :console => :environment do
  require 'pry'
  require 'readline'

  Pry.start
end

desc "Run unit tests"
require 'rspec/core/rake_task'
RSpec::Core::RakeTask.new do |t|
  t.pattern = Dir[File.expand_path('../spec/**/*_spec.rb', __FILE__)]
end
