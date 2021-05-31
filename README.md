1. Дефолтные значения: 1 cpu, 1024 mb ram, 64 gb hdd
2. Для увеличения ресурсов необходимо внести правки в Vagrantfile, например:
Vagrant.configure("2") do |config|
        config.vm.box = "bento/ubuntu-20.04"
config.vm.provider "virtualbox" do |v|
  v.memory = 2048
  v.cpus = 2
end
end
3. Команда HISTSIZE строка 1179; ignoreboth совмещает в себе две директивы ignorespace - не сохранять команды начинающиеся с пробелов и ignoredups - не сохранять повторяющиеся с последней командой строки
