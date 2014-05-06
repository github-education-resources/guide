require 'rubygems'
require 'bundler'
Bundler.require(:default)

require 'pry'

task :test do
  puts "Compiling and checking links..."
  # need to use a relative path
  proofer = MarkdownProofer.new('.')
  proofer.run
  if proofer.errors.any?
    puts proofer.errors.inspect
    puts "failure"
    raise "Failed! #{proofer.errors.join("\n")}"
  else
    puts "Success!"
  end
end

task default: :test
