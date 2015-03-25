# encoding: utf-8
$LOAD_PATH.unshift(File.join(File.dirname(__FILE__), 'tasks'))
$LOAD_PATH.unshift(File.dirname(__FILE__))

require 'rubygems'
require 'bundler'
require 'active_record'
require 'active_support/core_ext/string/strip'
require 'fileutils'
require 'yaml'
require 'erb'
require 'rakedb'

begin
  Bundler.setup(:default, :development)
rescue Bundler::BundlerError => e
  $stderr.puts e.message
  $stderr.puts "Run `bundle install` to install missing gems"
  exit e.status_code
end

require 'rake'

task :environment do
  ENV["RACK_ENV"] ||= 'development'
  require File.expand_path("../config/environment", __FILE__)
end
