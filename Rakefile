#!/usr/bin/env ruby
# -*- mode: ruby -*-

require 'rake'

desc 'Compile PDF'
task :compile do
  Dir.glob("*.tex").each do |f|
    sh "texi2pdf #{f}" do |(ok,res)|
      exit if not ok
    end
  end
end

task :default => [:compile]
