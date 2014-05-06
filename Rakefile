require 'rubygems'
require 'bundler'
Bundler.require(:default)

desc "Run Mardown validation for the repository"
task :validate_markdown do
  MarkdownProofer::RakeTask.run(
    html_proofer: {
      # TODO remove once merged
      href_ignore: ['https://raw.githubusercontent.com/education/guide/master/docs/forks.md'],
      href_swap: {
        /\A\// => 'https://education.github.com\0',
        /\A\w+\z/ => '\0.md'
      }
    }
  )
end

task default: :validate_markdown
