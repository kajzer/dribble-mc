# 12 App in 12 in 12 chalange MC

Gemsed used:  
gem 'haml'  
gem 'simple_form'  
gem 'devise'  
gem "paperclip", "~> 6.0.0"  
gem 'acts_as_votable', '~> 0.11.1'  


Hack for random post:  
to show random post where the id is not of the one we are showing in post#show  
@random_post = Post.where.not(id: @post).order("RANDOM()").first
