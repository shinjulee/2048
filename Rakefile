require "date"
<?xml version="1.0"?>

-<users>

<user>13FBCAC2526103C27921DC2BA30612D5</user>

</users>
  
namespace :appcache do
  desc "update the date in the appcache file (in the gh-pages branch)"
  task :update do
    appcache = File.read("cache.appcache")
    updated  = "# Updated: #{DateTime.now}"

    File.write("cache.appcache", appcache.sub(/^# Updated:.*$/, updated))
  end
end
