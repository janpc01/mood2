# Mood Board

A multimedia moodboard where you can upload audio and image files, or social-media embeds (Youtube, Instagram, X, Facebook, Pinterest), or Spotify embeds

A useful tool if you want to:

- Collect and organize media from multiple sources
- Share a moodboard with your friends.

## Development

### Techstack 
- Ruby 3 + Rails 7
- Hotwire ( Turbo + Stimulus )
- Tailwindcss
- NodeJS + ESbuild
- Postgresql 
- libvips ( image processing library )

### Setup
Install Ruby and Javascript dependencies:
```
bundle install
yarn install
```
Create and migration database: 
```
rails db:create
rails db:migrate
```
Start server:
```
./bin/dev
```

### Docker
```
docker-compose build

docker-compose run --rm web bin/rails db:create  
docker-compose run --rm web bin/rails db:migrate  
docker-compose run --rm web bin/rails db:seed  

docker-compose up 
```
