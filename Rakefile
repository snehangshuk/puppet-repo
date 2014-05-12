SSH = 'ssh -A -i ~/git/snehangshu/snehangshu.pem -l ubuntu'

desc "Run Puppet on ENV['CLIENT'}"
task :apply do
    client = ENV['CLIENT']
    sh "git push"
    sh "#{SSH} #{client} pull-updates"
end
