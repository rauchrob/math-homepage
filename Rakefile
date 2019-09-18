desc "build site locally"
task :build do
  sh "bundle exec jekyll build"
end

desc 'publish site'
task :deploy do
  user = 'robrauch'
  server = 'www.iaa.tu-bs.de'
  path = '~/www/'
  sh "rsync -rtzh --delete _site/ #{user}@#{server}:#{path}"
end
