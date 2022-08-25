require_relative './config/environment'
require 'sinatra/activerecord/rake'

# CREATE TASK WITHOUT DESCRIPTION

task :hello_world do 
    puts 'Hello World!'
end

# CREATE TASK WITH DESCRIPTION
desc 'creating a math_task'
task :output do 
    variation = (0.01/100) * 14000000
    puts variation
end

# ORGANIZE TASKS IN NAMESPACES
namespace :math_concepts do
    desc 'Find addition'
    task :addition, [:num1, :num2] do |t, args|
        puts (args[:num1].to_i + args[:num2].to_i)
    end
    desc 'Find subtraction'
    task :subtraction, [:num1, :num2] do |t, args|
        puts (args[:num1].to_i - args[:num2].to_i)
    end
    desc 'Find division'
    task :division, [:num1, :num2] do |t, args|
        puts (args[:num1].to_i / args[:num2].to_i)
    end
    desc 'Find multiplication'
    task :multiplication, [:num1, :num2] do |t, args|
        puts (args[:num1].to_i * args[:num2].to_i)
    end
end

