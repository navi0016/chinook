## README

[See instructions in Alexa.](https://alexa.bitmaker.co/cohorts/67/assignments/2038/latest)

1.  
  Artist.where(name:'Queen')

  Album.where('artist_id = ?','51')

2.
  MediaType.where('name = ?',"Protected MPEG-4 video file")

  Track.where('media_type_id = ?','3').count

3.
  Genre.where('name = ?','Hip Hop/Rap')
  Genre

4.
  Track.where('genre_id = ?','17').count

5.
  SELECT COUNT("tracks"."milliseconds") FROM "tracks"

6.
  Track.where('media_type_id = ?','1').maximum(:unit_price)

7.
  Track.order(:unit_price).where('media_type_id = ?','1').first.name

8.
  Artist.order(:created_at).limit(2).map { |k| k.name}

9.
  Genre.where('name = ?','Electronica/Dance')
  Track.order(:unit_price).where('genre_id = ?','15').first

10.

  Track.where(:genre_id => 15, :media_type_id => 1)
