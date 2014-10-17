task :default => :test

desc "Test the nanoc site"
task :test => :build do
  system "nanoc check --all"
end

desc "Build the nanoc site"
task :build => :clean do
  system "nanoc compile"
end

desc "Clean all build files and artifacts"
task :clean do
  system "rm -rf ./site ./tmp crash.log"
end

desc "View the nanoc site (localhost:3000)"
task :view do
  system "nanoc view"
end
