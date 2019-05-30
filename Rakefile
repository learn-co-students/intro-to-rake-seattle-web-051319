


namespace :greeting do
	#      should print out 'hello from Rake!'
desc 'outputs hello to the terminal'
  task :hello do
    puts "hello from Rake!"
  end

#      should print out 'hola de Rake!'
  desc 'outputs hola to the terminal'
  task :hola do
    puts "hola de Rake!"
  end
end



  desc 'outputs hola to the terminal'
  #    exists
  task :console do
    puts "hola de Rake!"
  end

namespace :db do
	#      invokes the :environment task as a dependency
  desc 'migrate changes to your database'
  task :migrate => :environment do
    Student.create_table
  end

#        create the students table in the database
  task :environment do
  require_relative './config/environment'
end

#      seeds the database with dummy data from a seed file
  desc 'seed the database with some dummy data'
  task :seed do
    require_relative './db/seeds.rb'
  end



end