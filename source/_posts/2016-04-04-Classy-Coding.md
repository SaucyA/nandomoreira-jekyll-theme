---
layout: post
title: "Classy Coding"
date: 2016-04-04 09:15
comments: true
description: "Object Oriented Programming"
categories:
- welcome
tags:
- welcome
---


Today’s blog post will teach you about the uses of Object Oriented design in Ruby coding. Below you will find an example of a Class with methods, instance variables, hashes and arrays.

	class Student
		def initialize
			log_in
		end

		def log_in
			puts "please enter your userename"
			@username = gets.chomp
			puts "please enter your password"
			@password = gets.chomp
		end

		def sign_up_for_classes
			puts "What classes do you want to take next year"
			@classes = []
			gets.chomp >> @classes
			gets.chomp >> @classes
			gets.chomp >> @classes
			gets.chomp >> @classes
			gets.chomp >> @classes

		end

		def check_homework
			@homework = hash.new
			@homework["4/3/16"] = "In math, Section 4.3.    In English, read chapeter 10"
			@homework["4/2/16"] = "In Science, do the lab   In spanish, finish the packet"
			puts @homework
		end

	end


	alden = Student.new


As you can see above, here is an example of Class coding in the Ruby language. The advantage is that it saves a lot of time(mlomnicki). Instead of having to write the individual code every time for each student in my example above, this class makes it easy for each student to login for themselves and subsequently pick their specific classes and view their upcoming assignments. The specific benefits that you can see in my example below is the use of instance variables (see as @______ below). These variables are special because they save but you can set the variable as what you want for each object in that class. Relating to my last point, the biggest perk of of using classes is the ease of making as many instances of the class. For example, in the above example at the bottom of the code when I wrote “alden = Student.new” I created a new student class named Alden. Now, I can login, sign up for classes and check Alden’s homework. These are the attributes of the class (Code Academy). I can make different attributes for each individual user. This means that if I were to create a new student, lets say Ben for example, the instance “Ben” will have a different username and password as well as the ability to choose his own classes, completely separate from Alden’s. Another advantage of using the Object Oriented Programming is the use of reader and writer methods. While my code does not feature any of these, these are easy way to input your attributes into your user and would be displayed as, “attr_reader” and “attr_writer” respectively, or to combine the two you would use “attr_accessor”. The only true disadvantage of the class is you can get lost a little but. When writing the code, you need to be cognizant of order of methods, and also putting your “end”s in the correct places. Truly, it is worth using and recommend you use it in your next time coding.

I hope you learned a lot today!! :)

Sources

http://mlomnicki.com/programming/ruby/2011/07/20/class-vs-instance-methods.html

http://ruby-doc.org/core-2.1.1/Hash.html (used in the coding)

https://www.codecademy.com/courses/ruby-beginner-enMFiQ6/0/1?curriculum_id=5059f8619189a5000201fbcb

