SSH = 'ssh -A -i ~/git/bitfield/bitfield.pem -l ubuntu'

desc "Run puppet on ENV['CLIENT']"
task: apply do
	client = ENV['CLIENT']
	ssh "git push"
	sh "#{SSH} #{client} pull-updates"
end
