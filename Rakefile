require 'rubygems'
require 'bundler'
Bundler.require(:default)

desc "Run Mardown validation for the repository"
task :validate_markdown do
  MarkdownProofer::RakeTask.run(
    html_proofer: {
      href_swap: {
        %r{\A/guide/(.*)\z} => '\1.md',
        %r{\A/} => 'https://education.github.com\0',
        %r{\Ahttps://raw.githubusercontent.com/education/guide/master/docs/(.*)\z} => '\1'
      }
    }
  )
end

task default: :validate_markdown
