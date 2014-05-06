require 'rubygems'
require 'bundler'
Bundler.require(:default)

desc "Run Mardown validation for the repository"
task :validate_markdown do
  MarkdownProofer::RakeTask.run(
    html_proofer: {
      href_swap: {
        /\A\// => 'https://education.github.com\0'
      }
    }
  )
end

task default: :validate_markdown
