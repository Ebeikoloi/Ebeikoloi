```python
!pip install spotipy
```

    Requirement already satisfied: spotipy in c:\users\hp\appdata\local\programs\python\python311\lib\site-packages (2.23.0)
    Requirement already satisfied: redis>=3.5.3 in c:\users\hp\appdata\local\programs\python\python311\lib\site-packages (from spotipy) (5.0.1)
    Requirement already satisfied: requests>=2.25.0 in c:\users\hp\appdata\local\programs\python\python311\lib\site-packages (from spotipy) (2.31.0)
    Requirement already satisfied: six>=1.15.0 in c:\users\hp\appdata\local\programs\python\python311\lib\site-packages (from spotipy) (1.16.0)
    Requirement already satisfied: urllib3>=1.26.0 in c:\users\hp\appdata\local\programs\python\python311\lib\site-packages (from spotipy) (2.0.4)
    Requirement already satisfied: charset-normalizer<4,>=2 in c:\users\hp\appdata\local\programs\python\python311\lib\site-packages (from requests>=2.25.0->spotipy) (3.2.0)
    Requirement already satisfied: idna<4,>=2.5 in c:\users\hp\appdata\local\programs\python\python311\lib\site-packages (from requests>=2.25.0->spotipy) (3.4)
    Requirement already satisfied: certifi>=2017.4.17 in c:\users\hp\appdata\local\programs\python\python311\lib\site-packages (from requests>=2.25.0->spotipy) (2023.7.22)
    

    
    [notice] A new release of pip is available: 23.2.1 -> 23.3.2
    [notice] To update, run: python.exe -m pip install --upgrade pip
    

    Requirement already satisfied: pandas in c:\users\hp\appdata\local\programs\python\python311\lib\site-packages (2.1.0)
    Requirement already satisfied: numpy>=1.23.2 in c:\users\hp\appdata\local\programs\python\python311\lib\site-packages (from pandas) (1.25.2)
    Requirement already satisfied: python-dateutil>=2.8.2 in c:\users\hp\appdata\local\programs\python\python311\lib\site-packages (from pandas) (2.8.2)
    Requirement already satisfied: pytz>=2020.1 in c:\users\hp\appdata\local\programs\python\python311\lib\site-packages (from pandas) (2023.3.post1)
    Requirement already satisfied: tzdata>=2022.1 in c:\users\hp\appdata\local\programs\python\python311\lib\site-packages (from pandas) (2023.3)
    Requirement already satisfied: six>=1.5 in c:\users\hp\appdata\local\programs\python\python311\lib\site-packages (from python-dateutil>=2.8.2->pandas) (1.16.0)
    

    
    [notice] A new release of pip is available: 23.2.1 -> 23.3.2
    [notice] To update, run: python.exe -m pip install --upgrade pip
    


```python
pip install spotipy --upgrade
```

    Requirement already satisfied: spotipy in c:\users\hp\appdata\local\programs\python\python311\lib\site-packages (2.23.0)Note: you may need to restart the kernel to use updated packages.
    
    Requirement already satisfied: redis>=3.5.3 in c:\users\hp\appdata\local\programs\python\python311\lib\site-packages (from spotipy) (5.0.1)
    Requirement already satisfied: requests>=2.25.0 in c:\users\hp\appdata\local\programs\python\python311\lib\site-packages (from spotipy) (2.31.0)
    Requirement already satisfied: six>=1.15.0 in c:\users\hp\appdata\local\programs\python\python311\lib\site-packages (from spotipy) (1.16.0)
    Requirement already satisfied: urllib3>=1.26.0 in c:\users\hp\appdata\local\programs\python\python311\lib\site-packages (from spotipy) (2.0.4)
    Requirement already satisfied: charset-normalizer<4,>=2 in c:\users\hp\appdata\local\programs\python\python311\lib\site-packages (from requests>=2.25.0->spotipy) (3.2.0)
    Requirement already satisfied: idna<4,>=2.5 in c:\users\hp\appdata\local\programs\python\python311\lib\site-packages (from requests>=2.25.0->spotipy) (3.4)
    Requirement already satisfied: certifi>=2017.4.17 in c:\users\hp\appdata\local\programs\python\python311\lib\site-packages (from requests>=2.25.0->spotipy) (2023.7.22)
    

    
    [notice] A new release of pip is available: 23.2.1 -> 23.3.2
    [notice] To update, run: python.exe -m pip install --upgrade pip
    


```python
pip install spotify
```

    Requirement already satisfied: spotify in c:\users\hp\appdata\local\programs\python\python311\lib\site-packages (0.10.2)Note: you may need to restart the kernel to use updated packages.
    

    
    [notice] A new release of pip is available: 23.2.1 -> 23.3.2
    [notice] To update, run: python.exe -m pip install --upgrade pip
    

    
    Requirement already satisfied: aiohttp<4.0,>=3.6 in c:\users\hp\appdata\local\programs\python\python311\lib\site-packages (from spotify) (3.9.1)
    Requirement already satisfied: backoff<2.0.0,>=1.10.0 in c:\users\hp\appdata\local\programs\python\python311\lib\site-packages (from spotify) (1.11.1)
    Requirement already satisfied: attrs>=17.3.0 in c:\users\hp\appdata\local\programs\python\python311\lib\site-packages (from aiohttp<4.0,>=3.6->spotify) (23.1.0)
    Requirement already satisfied: multidict<7.0,>=4.5 in c:\users\hp\appdata\local\programs\python\python311\lib\site-packages (from aiohttp<4.0,>=3.6->spotify) (6.0.4)
    Requirement already satisfied: yarl<2.0,>=1.0 in c:\users\hp\appdata\local\programs\python\python311\lib\site-packages (from aiohttp<4.0,>=3.6->spotify) (1.9.4)
    Requirement already satisfied: frozenlist>=1.1.1 in c:\users\hp\appdata\local\programs\python\python311\lib\site-packages (from aiohttp<4.0,>=3.6->spotify) (1.4.1)
    Requirement already satisfied: aiosignal>=1.1.2 in c:\users\hp\appdata\local\programs\python\python311\lib\site-packages (from aiohttp<4.0,>=3.6->spotify) (1.3.1)
    Requirement already satisfied: idna>=2.0 in c:\users\hp\appdata\local\programs\python\python311\lib\site-packages (from yarl<2.0,>=1.0->aiohttp<4.0,>=3.6->spotify) (3.4)
    


```python
import spotipy
from spotipy.oauth2 import SpotifyClientCredentials
import pandas as pd
```


```python
client_credentials_manager = SpotifyClientCredentials(client_id = 'aba2da3039af40be8878f4e93f0056d0', client_secret = 'a39aba3cd14f4e4ba42880c002407634') # for authentication
```


```python
sp = spotipy.Spotify(client_credentials_manager = client_credentials_manager) #creating sotify object so that we can extract data from it.This Code is for authorisation to download data
```


```python
sp 
```




    <spotipy.client.Spotify at 0x23bff9bab90>




```python
play_list_link = 'https://open.spotify.com/playlist/37i9dQZF1E4wl2HLNaYsgY'
```


```python
play_list_link
```




    'https://open.spotify.com/playlist/37i9dQZF1E4wl2HLNaYsgY'




```python
playlist_URL = play_list_link.split('/')[-1].split('?')[0]
```


```python
play_list_link
```




    'https://open.spotify.com/playlist/37i9dQZF1E4wl2HLNaYsgY'




```python
data = sp.playlist_tracks(playlist_URL) # it gives us a  json data 
```


```python
data['items'][0]['track']['album']['id']
```




    '1JzjwUKkPsdHg1SQ7qa5hc'




```python
data['items'][0]['track']['album']['release_date']
```




    '2023-08-24'




```python
data['items'][0]['track']['album']['total_tracks']
```




    15




```python
data['items'][0]['track']['album']['external_urls']['spotify']
```




    'https://open.spotify.com/album/1JzjwUKkPsdHg1SQ7qa5hc'




```python
# the above code was used to extract the indivual data metrics. in the next step we are going to optimise our code
```


```python
for row in data['items']:
    album_id = row['track']['album']['id']
    album_name = row['track']['album']['name']
    album_release_date = row['track']['album']['release_date']
    album_total_tracks = row['track']['album']['total_tracks']
    album_external_urls = row['track']['album']['external_urls']['spotify']
    print(album_name)
```


```python
# we need to convert this list into dictionary so we can create data frame
```


```python
for row in data['items']:
    album_id = row['track']['album']['id']
    album_name = row['track']['album']['name']
    album_release_date = row['track']['album']['release_date']
    album_total_tracks = row['track']['album']['total_tracks']
    album_external_urls = row['track']['album']['external_urls']['spotify']
    album_element = {'album_id':album_id,'album_name': album_name,'album_release_date':album_release_date,'album_total_tracks':album_total_tracks,'album_external_urls':album_external_urls}
    print(album_element)
```


```python
album_list = []
for row in data['items']:
    album_id = row['track']['album']['id']
    album_name = row['track']['album']['name']
    album_release_date = row['track']['album']['release_date']
    album_total_tracks = row['track']['album']['total_tracks']
    album_external_urls = row['track']['album']['external_urls']['spotify']
    album_element = {'album_id':album_id,'album_name': album_name,'album_release_date':album_release_date,'album_total_tracks':album_total_tracks,'album_external_urls':album_external_urls}
    album_list.append(album_element)
```


```python
album_list
```


```python
artist_list = []
for row in data['items']:
    for key, value in row.items():
        if key == 'track':
            for artist in value['artists']:
                artist_dict = {'artist_id':artist['id'], 'artist_name': artist['name'], 'external_urls':artist['href']}
                artist_list.append(artist_dict)
```


```python
artist_list
```


```python
song_list = []
for row in data['items']:
    song_id = row['track']['id']
    song_name = row['track']['name']
    song_duration = row['track']['duration_ms']
    song_url = row['track']['external_urls']['spotify']
    song_popularity = row['track']['popularity']
    song_added = row['added_at']
    album_id = row['track']['album']['id']
    artist_id = row['track']['album']['artists'][0]['id']
    song_element = {'song_id':song_id,'song_name': song_name,'duration_ms':song_duration,
                    'song_url':song_url,
                    'popularity':song_popularity,
                    'song_added':song_added,
                    'album_id':album_id,
                    'artist_id':artist_id
                   }
    song_list.append(song_element)
```


```python
song_list
```




    [{'song_id': '4RoKNqyZ9622tcAeNPNv5k',
      'song_name': 'City Boys',
      'duration_ms': 153346,
      'song_url': 'https://open.spotify.com/track/4RoKNqyZ9622tcAeNPNv5k',
      'popularity': 81,
      'song_added': '1970-01-01T00:00:00Z',
      'album_id': '1JzjwUKkPsdHg1SQ7qa5hc',
      'artist_id': '3wcj11K77LjEY1PkEazffa'},
     {'song_id': '5aIVCx5tnk0ntmdiinnYvw',
      'song_name': 'Water',
      'duration_ms': 200255,
      'song_url': 'https://open.spotify.com/track/5aIVCx5tnk0ntmdiinnYvw',
      'popularity': 94,
      'song_added': '1970-01-01T00:00:00Z',
      'album_id': '22sXXkKgjEuawIFL1e1tRw',
      'artist_id': '3SozjO3Lat463tQICI9LcE'},
     {'song_id': '6TTR7tXftck5lU7BPRY7bV',
      'song_name': 'Santorini Coffee',
      'duration_ms': 134365,
      'song_url': 'https://open.spotify.com/track/6TTR7tXftck5lU7BPRY7bV',
      'popularity': 71,
      'song_added': '1970-01-01T00:00:00Z',
      'album_id': '4np0ohQb06VAAitOpk3Rt4',
      'artist_id': '4Xj0nxVO4r7PLEaw7LRiBa'},
     {'song_id': '1eldTykrnkEBLX41bk5eMw',
      'song_name': 'Petit génie',
      'duration_ms': 217259,
      'song_url': 'https://open.spotify.com/track/1eldTykrnkEBLX41bk5eMw',
      'popularity': 80,
      'song_added': '1970-01-01T00:00:00Z',
      'album_id': '4Ta3fRzeMUtQlQrrcn1cuE',
      'artist_id': '6L8y2rKomt32RmT4wfwZS7'},
     {'song_id': '2FDTHlrBguDzQkp7PVj16Q',
      'song_name': 'Sprinter',
      'duration_ms': 229133,
      'song_url': 'https://open.spotify.com/track/2FDTHlrBguDzQkp7PVj16Q',
      'popularity': 89,
      'song_added': '1970-01-01T00:00:00Z',
      'album_id': '5l0QlaI3wdZpE7ggoO5Rwg',
      'artist_id': '6Ip8FS7vWT1uKkJSweANQK'},
     {'song_id': '5YbPxJwPfrj7uswNwoF1pJ',
      'song_name': 'Last Last',
      'duration_ms': 172342,
      'song_url': 'https://open.spotify.com/track/5YbPxJwPfrj7uswNwoF1pJ',
      'popularity': 79,
      'song_added': '1970-01-01T00:00:00Z',
      'album_id': '6kgDkAupBVRSqbJPUaTJwQ',
      'artist_id': '3wcj11K77LjEY1PkEazffa'},
     {'song_id': '0TZMDJP2MrGTSmWqUnswUh',
      'song_name': 'Shu-Peru',
      'duration_ms': 139377,
      'song_url': 'https://open.spotify.com/track/0TZMDJP2MrGTSmWqUnswUh',
      'popularity': 63,
      'song_added': '1970-01-01T00:00:00Z',
      'album_id': '2gbx0YcLDduf3oqujoq1fI',
      'artist_id': '1X6cBGnXpEpN7CmflLKmLV'},
     {'song_id': '6BWgLorAwF17ofyu8361HM',
      'song_name': 'Cast',
      'duration_ms': 129123,
      'song_url': 'https://open.spotify.com/track/6BWgLorAwF17ofyu8361HM',
      'popularity': 72,
      'song_added': '1970-01-01T00:00:00Z',
      'album_id': '14VJEhvxRCOsNtcwjjBxwR',
      'artist_id': '4TKhxSkqClXrdtUWgKqHVU'},
     {'song_id': '1wADwLSkYhrSmy4vdy6BRn',
      'song_name': 'soso',
      'duration_ms': 183056,
      'song_url': 'https://open.spotify.com/track/1wADwLSkYhrSmy4vdy6BRn',
      'popularity': 76,
      'song_added': '1970-01-01T00:00:00Z',
      'album_id': '5NLjxx8nRy9ooUmgpOvfem',
      'artist_id': '5yOvAmpIR7hVxiS6Ls5DPO'},
     {'song_id': '30RBuEKVJ2UXimaPtwAEIa',
      'song_name': 'Sans effet',
      'duration_ms': 160530,
      'song_url': 'https://open.spotify.com/track/30RBuEKVJ2UXimaPtwAEIa',
      'popularity': 61,
      'song_added': '1970-01-01T00:00:00Z',
      'album_id': '1uPEctEKBVjCRO5iGsya3b',
      'artist_id': '7gU9VyFRN3JWPJ5oHOil60'},
     {'song_id': '3sEcJ4mGZ9srlXdG7G2HK1',
      'song_name': 'Pull Up',
      'duration_ms': 187866,
      'song_url': 'https://open.spotify.com/track/3sEcJ4mGZ9srlXdG7G2HK1',
      'popularity': 51,
      'song_added': '1970-01-01T00:00:00Z',
      'album_id': '34vlTd4355ddD4q9pPsoqF',
      'artist_id': '3wcj11K77LjEY1PkEazffa'},
     {'song_id': '2WigMwGJysIh9fRnSJvpjn',
      'song_name': 'KU LO SA - A COLORS SHOW',
      'duration_ms': 147580,
      'song_url': 'https://open.spotify.com/track/2WigMwGJysIh9fRnSJvpjn',
      'popularity': 77,
      'song_added': '1970-01-01T00:00:00Z',
      'album_id': '36bNKiiUjxUCaAO7QtUVfi',
      'artist_id': '3WTrdbZU99dgTtt3ZkyamT'},
     {'song_id': '6nnZHjSHt0ZNtx4bIUky9P',
      'song_name': 'Boys Are Bad',
      'duration_ms': 137000,
      'song_url': 'https://open.spotify.com/track/6nnZHjSHt0ZNtx4bIUky9P',
      'popularity': 64,
      'song_added': '1970-01-01T00:00:00Z',
      'album_id': '17HtAdJO3qQzLJDf9GAePl',
      'artist_id': '1X6cBGnXpEpN7CmflLKmLV'},
     {'song_id': '6g8Ztyoym7VNLEzl8alsJK',
      'song_name': 'Move',
      'duration_ms': 150491,
      'song_url': 'https://open.spotify.com/track/6g8Ztyoym7VNLEzl8alsJK',
      'popularity': 57,
      'song_added': '1970-01-01T00:00:00Z',
      'album_id': '3Nt7p3GrkB4QeT1AKONY8U',
      'artist_id': '68R39izwNAztATrXMOqkJS'},
     {'song_id': '1iBWjQ9af9NnUd5xnQDB3k',
      'song_name': 'Charm',
      'duration_ms': 204750,
      'song_url': 'https://open.spotify.com/track/1iBWjQ9af9NnUd5xnQDB3k',
      'popularity': 74,
      'song_added': '1970-01-01T00:00:00Z',
      'album_id': '0nayxjaX54Frd7GsZq6Pbs',
      'artist_id': '46pWGuE3dSwY3bMMXGBvVS'},
     {'song_id': '6S9QZ8QTN5oOUChcYWChnK',
      'song_name': 'Shabba Madda Pot',
      'duration_ms': 142978,
      'song_url': 'https://open.spotify.com/track/6S9QZ8QTN5oOUChcYWChnK',
      'popularity': 61,
      'song_added': '1970-01-01T00:00:00Z',
      'album_id': '6blB91ubI6Ul0TFz6X2Non',
      'artist_id': '28UDeKu2FPrU0T7dpUiSGY'},
     {'song_id': '3a7ziOOO3Cbuv6BMXrj0wU',
      'song_name': 'Killin Dem (feat. Zlatan)',
      'duration_ms': 221100,
      'song_url': 'https://open.spotify.com/track/3a7ziOOO3Cbuv6BMXrj0wU',
      'popularity': 50,
      'song_added': '1970-01-01T00:00:00Z',
      'album_id': '34vlTd4355ddD4q9pPsoqF',
      'artist_id': '3wcj11K77LjEY1PkEazffa'},
     {'song_id': '0TTOsyDKykWhCh3qDd9wMY',
      'song_name': 'Talibans',
      'duration_ms': 188737,
      'song_url': 'https://open.spotify.com/track/0TTOsyDKykWhCh3qDd9wMY',
      'popularity': 70,
      'song_added': '1970-01-01T00:00:00Z',
      'album_id': '6Ds8n0PlFxomLOtEHFwBeo',
      'artist_id': '3IDfJpj4YVkaBl7Dd52Pxv'},
     {'song_id': '3nT2nrfb3FMLg03W4mPaBl',
      'song_name': 'Cough (Odo)',
      'duration_ms': 176195,
      'song_url': 'https://open.spotify.com/track/3nT2nrfb3FMLg03W4mPaBl',
      'popularity': 68,
      'song_added': '1970-01-01T00:00:00Z',
      'album_id': '2gbx0YcLDduf3oqujoq1fI',
      'artist_id': '1X6cBGnXpEpN7CmflLKmLV'},
     {'song_id': '2kaH2Z8ezDUKf6fNw250rZ',
      'song_name': 'UNAVAILABLE (feat. Musa Keys)',
      'duration_ms': 169911,
      'song_url': 'https://open.spotify.com/track/2kaH2Z8ezDUKf6fNw250rZ',
      'popularity': 78,
      'song_added': '1970-01-01T00:00:00Z',
      'album_id': '6lI21W76LD0S3vC55GrfSS',
      'artist_id': '0Y3agQaa6g2r0YmHPOO9rh'},
     {'song_id': '3ibXZkzvCPZ6lWbfubSolQ',
      'song_name': 'THIS YEAR (Blessings)',
      'duration_ms': 126206,
      'song_url': 'https://open.spotify.com/track/3ibXZkzvCPZ6lWbfubSolQ',
      'popularity': 62,
      'song_added': '1970-01-01T00:00:00Z',
      'album_id': '5wyDRKWKtPq3znLWVOtUIk',
      'artist_id': '5c0lDrNyT2RnFhujZpPIas'},
     {'song_id': '1OGZU2zmK6x0UnM3yeZ4lR',
      'song_name': 'Apollo',
      'duration_ms': 170000,
      'song_url': 'https://open.spotify.com/track/1OGZU2zmK6x0UnM3yeZ4lR',
      'popularity': 65,
      'song_added': '1970-01-01T00:00:00Z',
      'album_id': '1oSN6MKvpXR5WOHnsPi05w',
      'artist_id': '1E5hfn5BduN2nnoZCJmUVG'},
     {'song_id': '4k4pdUWX8632g7yByxC3rS',
      'song_name': 'Sungba (feat. Burna Boy) - Remix',
      'duration_ms': 210000,
      'song_url': 'https://open.spotify.com/track/4k4pdUWX8632g7yByxC3rS',
      'popularity': 66,
      'song_added': '1970-01-01T00:00:00Z',
      'album_id': '0lzPMIAYhhUSD2BPT0VQWI',
      'artist_id': '3a1tBryiczPAZpgoZN9Rzg'},
     {'song_id': '73e0LixjWj3e8prfptVeGD',
      'song_name': 'More Life',
      'duration_ms': 92342,
      'song_url': 'https://open.spotify.com/track/73e0LixjWj3e8prfptVeGD',
      'popularity': 58,
      'song_added': '1970-01-01T00:00:00Z',
      'album_id': '26du6obYLeY1vf6xIJ1l0D',
      'artist_id': '3wcj11K77LjEY1PkEazffa'},
     {'song_id': '03DxO8kGNrEGr1VjPSdQs2',
      'song_name': 'Lie',
      'duration_ms': 156600,
      'song_url': 'https://open.spotify.com/track/03DxO8kGNrEGr1VjPSdQs2',
      'popularity': 66,
      'song_added': '1970-01-01T00:00:00Z',
      'album_id': '0uk18xBtNopYpvMT1t7BCU',
      'artist_id': '1X6cBGnXpEpN7CmflLKmLV'},
     {'song_id': '6z5y2kdxF4XrEVRFVqdGVL',
      'song_name': 'Asiwaju',
      'duration_ms': 216000,
      'song_url': 'https://open.spotify.com/track/6z5y2kdxF4XrEVRFVqdGVL',
      'popularity': 67,
      'song_added': '1970-01-01T00:00:00Z',
      'album_id': '676QN3uS7pzWA0Or87JTcN',
      'artist_id': '0a1SidMjD8D6EHvJph4n2H'},
     {'song_id': '6qk3jI8bKCgURI3h0d8zBZ',
      'song_name': 'Again',
      'duration_ms': 156083,
      'song_url': 'https://open.spotify.com/track/6qk3jI8bKCgURI3h0d8zBZ',
      'popularity': 71,
      'song_added': '1970-01-01T00:00:00Z',
      'album_id': '0ZdiHNx2h4QTKwfF7fEM8j',
      'artist_id': '1fYVmAFB7sC7eDoF3mJXla'},
     {'song_id': '2HfK1KumDffDWPZga46Hmw',
      'song_name': 'Sugarcane',
      'duration_ms': 156781,
      'song_url': 'https://open.spotify.com/track/2HfK1KumDffDWPZga46Hmw',
      'popularity': 53,
      'song_added': '1970-01-01T00:00:00Z',
      'album_id': '2e7UIUu34tdxKVkcTG3463',
      'artist_id': '6Z9Xe5mjocmPOhz2TLNrAi'},
     {'song_id': '2LqvzGaZniHiZ9CXhzkclD',
      'song_name': 'Kwaku The Traveller',
      'duration_ms': 185364,
      'song_url': 'https://open.spotify.com/track/2LqvzGaZniHiZ9CXhzkclD',
      'popularity': 59,
      'song_added': '1970-01-01T00:00:00Z',
      'album_id': '7mnGUuvsSbUHZdKkJYdmOg',
      'artist_id': '2LiqbH7OhqP0yuaG8VL1wJ'},
     {'song_id': '7rpWDu9GPlLxbLorYKVys7',
      'song_name': 'Gbona',
      'duration_ms': 187609,
      'song_url': 'https://open.spotify.com/track/7rpWDu9GPlLxbLorYKVys7',
      'popularity': 70,
      'song_added': '1970-01-01T00:00:00Z',
      'album_id': '34vlTd4355ddD4q9pPsoqF',
      'artist_id': '3wcj11K77LjEY1PkEazffa'},
     {'song_id': '3IQT2MM49GkXfHF9eemaw5',
      'song_name': 'Soweto',
      'duration_ms': 148000,
      'song_url': 'https://open.spotify.com/track/3IQT2MM49GkXfHF9eemaw5',
      'popularity': 75,
      'song_added': '1970-01-01T00:00:00Z',
      'album_id': '1oSN6MKvpXR5WOHnsPi05w',
      'artist_id': '1E5hfn5BduN2nnoZCJmUVG'},
     {'song_id': '36tVdsRWDbPBekxVYEWhph',
      'song_name': 'Buga (Lo Lo Lo)',
      'duration_ms': 183103,
      'song_url': 'https://open.spotify.com/track/36tVdsRWDbPBekxVYEWhph',
      'popularity': 63,
      'song_added': '1970-01-01T00:00:00Z',
      'album_id': '2gbx0YcLDduf3oqujoq1fI',
      'artist_id': '1X6cBGnXpEpN7CmflLKmLV'},
     {'song_id': '1YgIvHDTvi1vosins1jyAC',
      'song_name': 'Amapiano',
      'duration_ms': 165000,
      'song_url': 'https://open.spotify.com/track/1YgIvHDTvi1vosins1jyAC',
      'popularity': 70,
      'song_added': '1970-01-01T00:00:00Z',
      'album_id': '2O9VJaLSnwjZ2HPpMaVoPU',
      'artist_id': '3a1tBryiczPAZpgoZN9Rzg'},
     {'song_id': '10U0rbctNl1DWEuCn1ETm6',
      'song_name': '𝘠𝘚𝘓',
      'duration_ms': 173714,
      'song_url': 'https://open.spotify.com/track/10U0rbctNl1DWEuCn1ETm6',
      'popularity': 63,
      'song_added': '1970-01-01T00:00:00Z',
      'album_id': '2FA3MmXyGWjL0IhoCdktU1',
      'artist_id': '7dYb5EKtRnRaWM0GQ12cKC'},
     {'song_id': '3F6xtKBO2YixpP8lFJTiGo',
      'song_name': 'Konongo Zongo',
      'duration_ms': 161699,
      'song_url': 'https://open.spotify.com/track/3F6xtKBO2YixpP8lFJTiGo',
      'popularity': 59,
      'song_added': '1970-01-01T00:00:00Z',
      'album_id': '7mnGUuvsSbUHZdKkJYdmOg',
      'artist_id': '2LiqbH7OhqP0yuaG8VL1wJ'},
     {'song_id': '1WsIk6g7dD8LZouywnzGUb',
      'song_name': 'Talibans II - Bonus Track',
      'duration_ms': 176453,
      'song_url': 'https://open.spotify.com/track/1WsIk6g7dD8LZouywnzGUb',
      'popularity': 67,
      'song_added': '1970-01-01T00:00:00Z',
      'album_id': '1JzjwUKkPsdHg1SQ7qa5hc',
      'artist_id': '3wcj11K77LjEY1PkEazffa'},
     {'song_id': '4TaS4giQQK01vKzBB40AEY',
      'song_name': 'Us Against the World',
      'duration_ms': 139786,
      'song_url': 'https://open.spotify.com/track/4TaS4giQQK01vKzBB40AEY',
      'popularity': 72,
      'song_added': '1970-01-01T00:00:00Z',
      'album_id': '5m2xRmSB1D30YZHDHr8556',
      'artist_id': '33X2jfLSVyDevoksJjRZoS'},
     {'song_id': '1PJUwqQNNWerJeVYFm1GEO',
      'song_name': 'We Wan Comot',
      'duration_ms': 124868,
      'song_url': 'https://open.spotify.com/track/1PJUwqQNNWerJeVYFm1GEO',
      'popularity': 62,
      'song_added': '1970-01-01T00:00:00Z',
      'album_id': '17HtAdJO3qQzLJDf9GAePl',
      'artist_id': '1X6cBGnXpEpN7CmflLKmLV'},
     {'song_id': '09FcXaLu1BdrRNgxyBi6p5',
      'song_name': 'Meridian',
      'duration_ms': 255160,
      'song_url': 'https://open.spotify.com/track/09FcXaLu1BdrRNgxyBi6p5',
      'popularity': 78,
      'song_added': '1970-01-01T00:00:00Z',
      'album_id': '2iz7b9HLy5aQ81tsMyedNn',
      'artist_id': '6Ip8FS7vWT1uKkJSweANQK'},
     {'song_id': '1ZrkOlKJ9db1cHnL1xEyfd',
      'song_name': 'P A S C O M M E Ç A',
      'duration_ms': 178226,
      'song_url': 'https://open.spotify.com/track/1ZrkOlKJ9db1cHnL1xEyfd',
      'popularity': 69,
      'song_added': '1970-01-01T00:00:00Z',
      'album_id': '1uPEctEKBVjCRO5iGsya3b',
      'artist_id': '7gU9VyFRN3JWPJ5oHOil60'},
     {'song_id': '4DdaGKeVkjQbPHzpoHGafk',
      'song_name': 'Second Sermon - Remix',
      'duration_ms': 194863,
      'song_url': 'https://open.spotify.com/track/4DdaGKeVkjQbPHzpoHGafk',
      'popularity': 59,
      'song_added': '1970-01-01T00:00:00Z',
      'album_id': '7mnGUuvsSbUHZdKkJYdmOg',
      'artist_id': '2LiqbH7OhqP0yuaG8VL1wJ'},
     {'song_id': '3A17uQFJab0NDpyIeZAavF',
      'song_name': 'Big 7',
      'duration_ms': 143042,
      'song_url': 'https://open.spotify.com/track/3A17uQFJab0NDpyIeZAavF',
      'popularity': 67,
      'song_added': '1970-01-01T00:00:00Z',
      'album_id': '1JzjwUKkPsdHg1SQ7qa5hc',
      'artist_id': '3wcj11K77LjEY1PkEazffa'},
     {'song_id': '6kgaI3kHkqmRimeGQdS4Ga',
      'song_name': 'Who Told You (feat. Drake)',
      'duration_ms': 208920,
      'song_url': 'https://open.spotify.com/track/6kgaI3kHkqmRimeGQdS4Ga',
      'popularity': 70,
      'song_added': '1970-01-01T00:00:00Z',
      'album_id': '766bxryPZBL0hjz0KM6VUD',
      'artist_id': '2a0uxJgbvvIRI4GX8pYfcr'},
     {'song_id': '1DrfpnLvbwndPScRLwbUE0',
      'song_name': 'Pour Me Water',
      'duration_ms': 146399,
      'song_url': 'https://open.spotify.com/track/1DrfpnLvbwndPScRLwbUE0',
      'popularity': 64,
      'song_added': '1970-01-01T00:00:00Z',
      'album_id': '0uk18xBtNopYpvMT1t7BCU',
      'artist_id': '1X6cBGnXpEpN7CmflLKmLV'},
     {'song_id': '0QdQh3umB7stVOExuHlWvl',
      'song_name': 'DECLAN RICE',
      'duration_ms': 124000,
      'song_url': 'https://open.spotify.com/track/0QdQh3umB7stVOExuHlWvl',
      'popularity': 64,
      'song_added': '1970-01-01T00:00:00Z',
      'album_id': '6e1McsPwHgiySHVlpZRhFx',
      'artist_id': '3LOm0AZjpwVQebvkyanjDy'},
     {'song_id': '0SjQBdIddPvKSWxr8vk6QX',
      'song_name': 'Dumebi',
      'duration_ms': 179775,
      'song_url': 'https://open.spotify.com/track/0SjQBdIddPvKSWxr8vk6QX',
      'popularity': 67,
      'song_added': '1970-01-01T00:00:00Z',
      'album_id': '4l8Gg5qk0QodyJ12SNtdUf',
      'artist_id': '46pWGuE3dSwY3bMMXGBvVS'},
     {'song_id': '0FnoxHCkfmjr2kBDwos4OG',
      'song_name': 'Bella',
      'duration_ms': 146478,
      'song_url': 'https://open.spotify.com/track/0FnoxHCkfmjr2kBDwos4OG',
      'popularity': 54,
      'song_added': '1970-01-01T00:00:00Z',
      'album_id': '34UcYlaPC0yAo0FZV6xoHD',
      'artist_id': '2TwUVWFJs4LD0lOBbJXnNa'},
     {'song_id': '1PoJXULCvl03b1fiZmMxmd',
      'song_name': 'On the Low',
      'duration_ms': 185898,
      'song_url': 'https://open.spotify.com/track/1PoJXULCvl03b1fiZmMxmd',
      'popularity': 73,
      'song_added': '1970-01-01T00:00:00Z',
      'album_id': '34vlTd4355ddD4q9pPsoqF',
      'artist_id': '3wcj11K77LjEY1PkEazffa'},
     {'song_id': '3aJF7HsFOwuUAFOaRMQCxR',
      'song_name': 'Butta My Bread',
      'duration_ms': 148672,
      'song_url': 'https://open.spotify.com/track/3aJF7HsFOwuUAFOaRMQCxR',
      'popularity': 72,
      'song_added': '1970-01-01T00:00:00Z',
      'album_id': '3WlxlO16ydHEisWjriRpHk',
      'artist_id': '3gYUwwn7FiiBMKHe36OUaQ'},
     {'song_id': '5a8IYhZWozHBb0bmqbogyq',
      'song_name': 'RTID (Rich Till I Die)',
      'duration_ms': 172944,
      'song_url': 'https://open.spotify.com/track/5a8IYhZWozHBb0bmqbogyq',
      'popularity': 59,
      'song_added': '1970-01-01T00:00:00Z',
      'album_id': '2gbx0YcLDduf3oqujoq1fI',
      'artist_id': '1X6cBGnXpEpN7CmflLKmLV'}]




```python
#convert (album-list,song_list and artist_list) to DataFrame 
```


```python
album_df = pd.DataFrame.from_dict(album_list) 
song_df = pd.DataFrame.from_dict(song_list)
artist_df = pd.DataFrame.from_dict(artist_list)
```


```python
song_df
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>song_id</th>
      <th>song_name</th>
      <th>duration_ms</th>
      <th>song_url</th>
      <th>popularity</th>
      <th>song_added</th>
      <th>album_id</th>
      <th>artist_id</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>4RoKNqyZ9622tcAeNPNv5k</td>
      <td>City Boys</td>
      <td>153346</td>
      <td>https://open.spotify.com/track/4RoKNqyZ9622tcA...</td>
      <td>81</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>1JzjwUKkPsdHg1SQ7qa5hc</td>
      <td>3wcj11K77LjEY1PkEazffa</td>
    </tr>
    <tr>
      <th>1</th>
      <td>5aIVCx5tnk0ntmdiinnYvw</td>
      <td>Water</td>
      <td>200255</td>
      <td>https://open.spotify.com/track/5aIVCx5tnk0ntmd...</td>
      <td>94</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>22sXXkKgjEuawIFL1e1tRw</td>
      <td>3SozjO3Lat463tQICI9LcE</td>
    </tr>
    <tr>
      <th>2</th>
      <td>6TTR7tXftck5lU7BPRY7bV</td>
      <td>Santorini Coffee</td>
      <td>134365</td>
      <td>https://open.spotify.com/track/6TTR7tXftck5lU7...</td>
      <td>71</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>4np0ohQb06VAAitOpk3Rt4</td>
      <td>4Xj0nxVO4r7PLEaw7LRiBa</td>
    </tr>
    <tr>
      <th>3</th>
      <td>1eldTykrnkEBLX41bk5eMw</td>
      <td>Petit génie</td>
      <td>217259</td>
      <td>https://open.spotify.com/track/1eldTykrnkEBLX4...</td>
      <td>80</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>4Ta3fRzeMUtQlQrrcn1cuE</td>
      <td>6L8y2rKomt32RmT4wfwZS7</td>
    </tr>
    <tr>
      <th>4</th>
      <td>2FDTHlrBguDzQkp7PVj16Q</td>
      <td>Sprinter</td>
      <td>229133</td>
      <td>https://open.spotify.com/track/2FDTHlrBguDzQkp...</td>
      <td>89</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>5l0QlaI3wdZpE7ggoO5Rwg</td>
      <td>6Ip8FS7vWT1uKkJSweANQK</td>
    </tr>
    <tr>
      <th>5</th>
      <td>5YbPxJwPfrj7uswNwoF1pJ</td>
      <td>Last Last</td>
      <td>172342</td>
      <td>https://open.spotify.com/track/5YbPxJwPfrj7usw...</td>
      <td>79</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>6kgDkAupBVRSqbJPUaTJwQ</td>
      <td>3wcj11K77LjEY1PkEazffa</td>
    </tr>
    <tr>
      <th>6</th>
      <td>0TZMDJP2MrGTSmWqUnswUh</td>
      <td>Shu-Peru</td>
      <td>139377</td>
      <td>https://open.spotify.com/track/0TZMDJP2MrGTSmW...</td>
      <td>63</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>2gbx0YcLDduf3oqujoq1fI</td>
      <td>1X6cBGnXpEpN7CmflLKmLV</td>
    </tr>
    <tr>
      <th>7</th>
      <td>6BWgLorAwF17ofyu8361HM</td>
      <td>Cast</td>
      <td>129123</td>
      <td>https://open.spotify.com/track/6BWgLorAwF17ofy...</td>
      <td>72</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>14VJEhvxRCOsNtcwjjBxwR</td>
      <td>4TKhxSkqClXrdtUWgKqHVU</td>
    </tr>
    <tr>
      <th>8</th>
      <td>1wADwLSkYhrSmy4vdy6BRn</td>
      <td>soso</td>
      <td>183056</td>
      <td>https://open.spotify.com/track/1wADwLSkYhrSmy4...</td>
      <td>76</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>5NLjxx8nRy9ooUmgpOvfem</td>
      <td>5yOvAmpIR7hVxiS6Ls5DPO</td>
    </tr>
    <tr>
      <th>9</th>
      <td>30RBuEKVJ2UXimaPtwAEIa</td>
      <td>Sans effet</td>
      <td>160530</td>
      <td>https://open.spotify.com/track/30RBuEKVJ2UXima...</td>
      <td>61</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>1uPEctEKBVjCRO5iGsya3b</td>
      <td>7gU9VyFRN3JWPJ5oHOil60</td>
    </tr>
    <tr>
      <th>10</th>
      <td>3sEcJ4mGZ9srlXdG7G2HK1</td>
      <td>Pull Up</td>
      <td>187866</td>
      <td>https://open.spotify.com/track/3sEcJ4mGZ9srlXd...</td>
      <td>51</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>34vlTd4355ddD4q9pPsoqF</td>
      <td>3wcj11K77LjEY1PkEazffa</td>
    </tr>
    <tr>
      <th>11</th>
      <td>2WigMwGJysIh9fRnSJvpjn</td>
      <td>KU LO SA - A COLORS SHOW</td>
      <td>147580</td>
      <td>https://open.spotify.com/track/2WigMwGJysIh9fR...</td>
      <td>77</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>36bNKiiUjxUCaAO7QtUVfi</td>
      <td>3WTrdbZU99dgTtt3ZkyamT</td>
    </tr>
    <tr>
      <th>12</th>
      <td>6nnZHjSHt0ZNtx4bIUky9P</td>
      <td>Boys Are Bad</td>
      <td>137000</td>
      <td>https://open.spotify.com/track/6nnZHjSHt0ZNtx4...</td>
      <td>64</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>17HtAdJO3qQzLJDf9GAePl</td>
      <td>1X6cBGnXpEpN7CmflLKmLV</td>
    </tr>
    <tr>
      <th>13</th>
      <td>6g8Ztyoym7VNLEzl8alsJK</td>
      <td>Move</td>
      <td>150491</td>
      <td>https://open.spotify.com/track/6g8Ztyoym7VNLEz...</td>
      <td>57</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>3Nt7p3GrkB4QeT1AKONY8U</td>
      <td>68R39izwNAztATrXMOqkJS</td>
    </tr>
    <tr>
      <th>14</th>
      <td>1iBWjQ9af9NnUd5xnQDB3k</td>
      <td>Charm</td>
      <td>204750</td>
      <td>https://open.spotify.com/track/1iBWjQ9af9NnUd5...</td>
      <td>74</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>0nayxjaX54Frd7GsZq6Pbs</td>
      <td>46pWGuE3dSwY3bMMXGBvVS</td>
    </tr>
    <tr>
      <th>15</th>
      <td>6S9QZ8QTN5oOUChcYWChnK</td>
      <td>Shabba Madda Pot</td>
      <td>142978</td>
      <td>https://open.spotify.com/track/6S9QZ8QTN5oOUCh...</td>
      <td>61</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>6blB91ubI6Ul0TFz6X2Non</td>
      <td>28UDeKu2FPrU0T7dpUiSGY</td>
    </tr>
    <tr>
      <th>16</th>
      <td>3a7ziOOO3Cbuv6BMXrj0wU</td>
      <td>Killin Dem (feat. Zlatan)</td>
      <td>221100</td>
      <td>https://open.spotify.com/track/3a7ziOOO3Cbuv6B...</td>
      <td>50</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>34vlTd4355ddD4q9pPsoqF</td>
      <td>3wcj11K77LjEY1PkEazffa</td>
    </tr>
    <tr>
      <th>17</th>
      <td>0TTOsyDKykWhCh3qDd9wMY</td>
      <td>Talibans</td>
      <td>188737</td>
      <td>https://open.spotify.com/track/0TTOsyDKykWhCh3...</td>
      <td>70</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>6Ds8n0PlFxomLOtEHFwBeo</td>
      <td>3IDfJpj4YVkaBl7Dd52Pxv</td>
    </tr>
    <tr>
      <th>18</th>
      <td>3nT2nrfb3FMLg03W4mPaBl</td>
      <td>Cough (Odo)</td>
      <td>176195</td>
      <td>https://open.spotify.com/track/3nT2nrfb3FMLg03...</td>
      <td>68</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>2gbx0YcLDduf3oqujoq1fI</td>
      <td>1X6cBGnXpEpN7CmflLKmLV</td>
    </tr>
    <tr>
      <th>19</th>
      <td>2kaH2Z8ezDUKf6fNw250rZ</td>
      <td>UNAVAILABLE (feat. Musa Keys)</td>
      <td>169911</td>
      <td>https://open.spotify.com/track/2kaH2Z8ezDUKf6f...</td>
      <td>78</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>6lI21W76LD0S3vC55GrfSS</td>
      <td>0Y3agQaa6g2r0YmHPOO9rh</td>
    </tr>
    <tr>
      <th>20</th>
      <td>3ibXZkzvCPZ6lWbfubSolQ</td>
      <td>THIS YEAR (Blessings)</td>
      <td>126206</td>
      <td>https://open.spotify.com/track/3ibXZkzvCPZ6lWb...</td>
      <td>62</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>5wyDRKWKtPq3znLWVOtUIk</td>
      <td>5c0lDrNyT2RnFhujZpPIas</td>
    </tr>
    <tr>
      <th>21</th>
      <td>1OGZU2zmK6x0UnM3yeZ4lR</td>
      <td>Apollo</td>
      <td>170000</td>
      <td>https://open.spotify.com/track/1OGZU2zmK6x0UnM...</td>
      <td>65</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>1oSN6MKvpXR5WOHnsPi05w</td>
      <td>1E5hfn5BduN2nnoZCJmUVG</td>
    </tr>
    <tr>
      <th>22</th>
      <td>4k4pdUWX8632g7yByxC3rS</td>
      <td>Sungba (feat. Burna Boy) - Remix</td>
      <td>210000</td>
      <td>https://open.spotify.com/track/4k4pdUWX8632g7y...</td>
      <td>66</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>0lzPMIAYhhUSD2BPT0VQWI</td>
      <td>3a1tBryiczPAZpgoZN9Rzg</td>
    </tr>
    <tr>
      <th>23</th>
      <td>73e0LixjWj3e8prfptVeGD</td>
      <td>More Life</td>
      <td>92342</td>
      <td>https://open.spotify.com/track/73e0LixjWj3e8pr...</td>
      <td>58</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>26du6obYLeY1vf6xIJ1l0D</td>
      <td>3wcj11K77LjEY1PkEazffa</td>
    </tr>
    <tr>
      <th>24</th>
      <td>03DxO8kGNrEGr1VjPSdQs2</td>
      <td>Lie</td>
      <td>156600</td>
      <td>https://open.spotify.com/track/03DxO8kGNrEGr1V...</td>
      <td>66</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>0uk18xBtNopYpvMT1t7BCU</td>
      <td>1X6cBGnXpEpN7CmflLKmLV</td>
    </tr>
    <tr>
      <th>25</th>
      <td>6z5y2kdxF4XrEVRFVqdGVL</td>
      <td>Asiwaju</td>
      <td>216000</td>
      <td>https://open.spotify.com/track/6z5y2kdxF4XrEVR...</td>
      <td>67</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>676QN3uS7pzWA0Or87JTcN</td>
      <td>0a1SidMjD8D6EHvJph4n2H</td>
    </tr>
    <tr>
      <th>26</th>
      <td>6qk3jI8bKCgURI3h0d8zBZ</td>
      <td>Again</td>
      <td>156083</td>
      <td>https://open.spotify.com/track/6qk3jI8bKCgURI3...</td>
      <td>71</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>0ZdiHNx2h4QTKwfF7fEM8j</td>
      <td>1fYVmAFB7sC7eDoF3mJXla</td>
    </tr>
    <tr>
      <th>27</th>
      <td>2HfK1KumDffDWPZga46Hmw</td>
      <td>Sugarcane</td>
      <td>156781</td>
      <td>https://open.spotify.com/track/2HfK1KumDffDWPZ...</td>
      <td>53</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>2e7UIUu34tdxKVkcTG3463</td>
      <td>6Z9Xe5mjocmPOhz2TLNrAi</td>
    </tr>
    <tr>
      <th>28</th>
      <td>2LqvzGaZniHiZ9CXhzkclD</td>
      <td>Kwaku The Traveller</td>
      <td>185364</td>
      <td>https://open.spotify.com/track/2LqvzGaZniHiZ9C...</td>
      <td>59</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>7mnGUuvsSbUHZdKkJYdmOg</td>
      <td>2LiqbH7OhqP0yuaG8VL1wJ</td>
    </tr>
    <tr>
      <th>29</th>
      <td>7rpWDu9GPlLxbLorYKVys7</td>
      <td>Gbona</td>
      <td>187609</td>
      <td>https://open.spotify.com/track/7rpWDu9GPlLxbLo...</td>
      <td>70</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>34vlTd4355ddD4q9pPsoqF</td>
      <td>3wcj11K77LjEY1PkEazffa</td>
    </tr>
    <tr>
      <th>30</th>
      <td>3IQT2MM49GkXfHF9eemaw5</td>
      <td>Soweto</td>
      <td>148000</td>
      <td>https://open.spotify.com/track/3IQT2MM49GkXfHF...</td>
      <td>75</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>1oSN6MKvpXR5WOHnsPi05w</td>
      <td>1E5hfn5BduN2nnoZCJmUVG</td>
    </tr>
    <tr>
      <th>31</th>
      <td>36tVdsRWDbPBekxVYEWhph</td>
      <td>Buga (Lo Lo Lo)</td>
      <td>183103</td>
      <td>https://open.spotify.com/track/36tVdsRWDbPBekx...</td>
      <td>63</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>2gbx0YcLDduf3oqujoq1fI</td>
      <td>1X6cBGnXpEpN7CmflLKmLV</td>
    </tr>
    <tr>
      <th>32</th>
      <td>1YgIvHDTvi1vosins1jyAC</td>
      <td>Amapiano</td>
      <td>165000</td>
      <td>https://open.spotify.com/track/1YgIvHDTvi1vosi...</td>
      <td>70</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>2O9VJaLSnwjZ2HPpMaVoPU</td>
      <td>3a1tBryiczPAZpgoZN9Rzg</td>
    </tr>
    <tr>
      <th>33</th>
      <td>10U0rbctNl1DWEuCn1ETm6</td>
      <td>𝘠𝘚𝘓</td>
      <td>173714</td>
      <td>https://open.spotify.com/track/10U0rbctNl1DWEu...</td>
      <td>63</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>2FA3MmXyGWjL0IhoCdktU1</td>
      <td>7dYb5EKtRnRaWM0GQ12cKC</td>
    </tr>
    <tr>
      <th>34</th>
      <td>3F6xtKBO2YixpP8lFJTiGo</td>
      <td>Konongo Zongo</td>
      <td>161699</td>
      <td>https://open.spotify.com/track/3F6xtKBO2YixpP8...</td>
      <td>59</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>7mnGUuvsSbUHZdKkJYdmOg</td>
      <td>2LiqbH7OhqP0yuaG8VL1wJ</td>
    </tr>
    <tr>
      <th>35</th>
      <td>1WsIk6g7dD8LZouywnzGUb</td>
      <td>Talibans II - Bonus Track</td>
      <td>176453</td>
      <td>https://open.spotify.com/track/1WsIk6g7dD8LZou...</td>
      <td>67</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>1JzjwUKkPsdHg1SQ7qa5hc</td>
      <td>3wcj11K77LjEY1PkEazffa</td>
    </tr>
    <tr>
      <th>36</th>
      <td>4TaS4giQQK01vKzBB40AEY</td>
      <td>Us Against the World</td>
      <td>139786</td>
      <td>https://open.spotify.com/track/4TaS4giQQK01vKz...</td>
      <td>72</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>5m2xRmSB1D30YZHDHr8556</td>
      <td>33X2jfLSVyDevoksJjRZoS</td>
    </tr>
    <tr>
      <th>37</th>
      <td>1PJUwqQNNWerJeVYFm1GEO</td>
      <td>We Wan Comot</td>
      <td>124868</td>
      <td>https://open.spotify.com/track/1PJUwqQNNWerJeV...</td>
      <td>62</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>17HtAdJO3qQzLJDf9GAePl</td>
      <td>1X6cBGnXpEpN7CmflLKmLV</td>
    </tr>
    <tr>
      <th>38</th>
      <td>09FcXaLu1BdrRNgxyBi6p5</td>
      <td>Meridian</td>
      <td>255160</td>
      <td>https://open.spotify.com/track/09FcXaLu1BdrRNg...</td>
      <td>78</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>2iz7b9HLy5aQ81tsMyedNn</td>
      <td>6Ip8FS7vWT1uKkJSweANQK</td>
    </tr>
    <tr>
      <th>39</th>
      <td>1ZrkOlKJ9db1cHnL1xEyfd</td>
      <td>P A S C O M M E Ç A</td>
      <td>178226</td>
      <td>https://open.spotify.com/track/1ZrkOlKJ9db1cHn...</td>
      <td>69</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>1uPEctEKBVjCRO5iGsya3b</td>
      <td>7gU9VyFRN3JWPJ5oHOil60</td>
    </tr>
    <tr>
      <th>40</th>
      <td>4DdaGKeVkjQbPHzpoHGafk</td>
      <td>Second Sermon - Remix</td>
      <td>194863</td>
      <td>https://open.spotify.com/track/4DdaGKeVkjQbPHz...</td>
      <td>59</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>7mnGUuvsSbUHZdKkJYdmOg</td>
      <td>2LiqbH7OhqP0yuaG8VL1wJ</td>
    </tr>
    <tr>
      <th>41</th>
      <td>3A17uQFJab0NDpyIeZAavF</td>
      <td>Big 7</td>
      <td>143042</td>
      <td>https://open.spotify.com/track/3A17uQFJab0NDpy...</td>
      <td>67</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>1JzjwUKkPsdHg1SQ7qa5hc</td>
      <td>3wcj11K77LjEY1PkEazffa</td>
    </tr>
    <tr>
      <th>42</th>
      <td>6kgaI3kHkqmRimeGQdS4Ga</td>
      <td>Who Told You (feat. Drake)</td>
      <td>208920</td>
      <td>https://open.spotify.com/track/6kgaI3kHkqmRime...</td>
      <td>70</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>766bxryPZBL0hjz0KM6VUD</td>
      <td>2a0uxJgbvvIRI4GX8pYfcr</td>
    </tr>
    <tr>
      <th>43</th>
      <td>1DrfpnLvbwndPScRLwbUE0</td>
      <td>Pour Me Water</td>
      <td>146399</td>
      <td>https://open.spotify.com/track/1DrfpnLvbwndPSc...</td>
      <td>64</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>0uk18xBtNopYpvMT1t7BCU</td>
      <td>1X6cBGnXpEpN7CmflLKmLV</td>
    </tr>
    <tr>
      <th>44</th>
      <td>0QdQh3umB7stVOExuHlWvl</td>
      <td>DECLAN RICE</td>
      <td>124000</td>
      <td>https://open.spotify.com/track/0QdQh3umB7stVOE...</td>
      <td>64</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>6e1McsPwHgiySHVlpZRhFx</td>
      <td>3LOm0AZjpwVQebvkyanjDy</td>
    </tr>
    <tr>
      <th>45</th>
      <td>0SjQBdIddPvKSWxr8vk6QX</td>
      <td>Dumebi</td>
      <td>179775</td>
      <td>https://open.spotify.com/track/0SjQBdIddPvKSWx...</td>
      <td>67</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>4l8Gg5qk0QodyJ12SNtdUf</td>
      <td>46pWGuE3dSwY3bMMXGBvVS</td>
    </tr>
    <tr>
      <th>46</th>
      <td>0FnoxHCkfmjr2kBDwos4OG</td>
      <td>Bella</td>
      <td>146478</td>
      <td>https://open.spotify.com/track/0FnoxHCkfmjr2kB...</td>
      <td>54</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>34UcYlaPC0yAo0FZV6xoHD</td>
      <td>2TwUVWFJs4LD0lOBbJXnNa</td>
    </tr>
    <tr>
      <th>47</th>
      <td>1PoJXULCvl03b1fiZmMxmd</td>
      <td>On the Low</td>
      <td>185898</td>
      <td>https://open.spotify.com/track/1PoJXULCvl03b1f...</td>
      <td>73</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>34vlTd4355ddD4q9pPsoqF</td>
      <td>3wcj11K77LjEY1PkEazffa</td>
    </tr>
    <tr>
      <th>48</th>
      <td>3aJF7HsFOwuUAFOaRMQCxR</td>
      <td>Butta My Bread</td>
      <td>148672</td>
      <td>https://open.spotify.com/track/3aJF7HsFOwuUAFO...</td>
      <td>72</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>3WlxlO16ydHEisWjriRpHk</td>
      <td>3gYUwwn7FiiBMKHe36OUaQ</td>
    </tr>
    <tr>
      <th>49</th>
      <td>5a8IYhZWozHBb0bmqbogyq</td>
      <td>RTID (Rich Till I Die)</td>
      <td>172944</td>
      <td>https://open.spotify.com/track/5a8IYhZWozHBb0b...</td>
      <td>59</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>2gbx0YcLDduf3oqujoq1fI</td>
      <td>1X6cBGnXpEpN7CmflLKmLV</td>
    </tr>
  </tbody>
</table>
</div>




```python
album_df.info()
```

    <class 'pandas.core.frame.DataFrame'>
    Index: 36 entries, 0 to 48
    Data columns (total 5 columns):
     #   Column               Non-Null Count  Dtype 
    ---  ------               --------------  ----- 
     0   album_id             36 non-null     object
     1   album_name           36 non-null     object
     2   album_release_date   36 non-null     object
     3   album_total_tracks   36 non-null     int64 
     4   album_external_urls  36 non-null     object
    dtypes: int64(1), object(4)
    memory usage: 1.7+ KB
    


```python
# let see if all the indivual fields has the right data types
```


```python
album_df.info()
```

    <class 'pandas.core.frame.DataFrame'>
    RangeIndex: 50 entries, 0 to 49
    Data columns (total 5 columns):
     #   Column               Non-Null Count  Dtype 
    ---  ------               --------------  ----- 
     0   album_id             50 non-null     object
     1   album_name           50 non-null     object
     2   album_release_date   50 non-null     object
     3   album_total_tracks   50 non-null     int64 
     4   album_external_urls  50 non-null     object
    dtypes: int64(1), object(4)
    memory usage: 2.1+ KB
    


```python
# to remove duplicates
```


```python
album_df = album_df.drop_duplicates(subset = ['album_id']) 
artist_df =artist_df.drop_duplicates(subset = ['artist_id'])
```


```python
# song_df = song_df.drop_duplicates(subset = ['song_id']), there is no need to drop duplicate for the songs
```


```python
album_df
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>album_id</th>
      <th>album_name</th>
      <th>album_release_date</th>
      <th>album_total_tracks</th>
      <th>album_external_urls</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>1JzjwUKkPsdHg1SQ7qa5hc</td>
      <td>I Told Them...</td>
      <td>2023-08-24</td>
      <td>15</td>
      <td>https://open.spotify.com/track/4RoKNqyZ9622tcA...</td>
    </tr>
    <tr>
      <th>1</th>
      <td>22sXXkKgjEuawIFL1e1tRw</td>
      <td>Water</td>
      <td>2023-07-28</td>
      <td>1</td>
      <td>https://open.spotify.com/track/5aIVCx5tnk0ntmd...</td>
    </tr>
    <tr>
      <th>2</th>
      <td>4np0ohQb06VAAitOpk3Rt4</td>
      <td>THENIGHTISYOUNG.</td>
      <td>2019-02-22</td>
      <td>4</td>
      <td>https://open.spotify.com/track/6TTR7tXftck5lU7...</td>
    </tr>
    <tr>
      <th>3</th>
      <td>4Ta3fRzeMUtQlQrrcn1cuE</td>
      <td>Petit génie</td>
      <td>2023-08-04</td>
      <td>1</td>
      <td>https://open.spotify.com/track/1eldTykrnkEBLX4...</td>
    </tr>
    <tr>
      <th>4</th>
      <td>5l0QlaI3wdZpE7ggoO5Rwg</td>
      <td>Sprinter</td>
      <td>2023-06-01</td>
      <td>1</td>
      <td>https://open.spotify.com/track/2FDTHlrBguDzQkp...</td>
    </tr>
    <tr>
      <th>5</th>
      <td>6kgDkAupBVRSqbJPUaTJwQ</td>
      <td>Love, Damini</td>
      <td>2022-07-07</td>
      <td>19</td>
      <td>https://open.spotify.com/track/5YbPxJwPfrj7usw...</td>
    </tr>
    <tr>
      <th>6</th>
      <td>2gbx0YcLDduf3oqujoq1fI</td>
      <td>Maverick</td>
      <td>2023-07-27</td>
      <td>20</td>
      <td>https://open.spotify.com/track/0TZMDJP2MrGTSmW...</td>
    </tr>
    <tr>
      <th>7</th>
      <td>14VJEhvxRCOsNtcwjjBxwR</td>
      <td>Presido La Pluto</td>
      <td>2023-11-10</td>
      <td>13</td>
      <td>https://open.spotify.com/track/6BWgLorAwF17ofy...</td>
    </tr>
    <tr>
      <th>8</th>
      <td>5NLjxx8nRy9ooUmgpOvfem</td>
      <td>Boy Alone</td>
      <td>2022-07-14</td>
      <td>14</td>
      <td>https://open.spotify.com/track/1wADwLSkYhrSmy4...</td>
    </tr>
    <tr>
      <th>9</th>
      <td>1uPEctEKBVjCRO5iGsya3b</td>
      <td>Fleur froide - Second état : la cristallisation</td>
      <td>2021-11-19</td>
      <td>41</td>
      <td>https://open.spotify.com/track/30RBuEKVJ2UXima...</td>
    </tr>
    <tr>
      <th>10</th>
      <td>34vlTd4355ddD4q9pPsoqF</td>
      <td>African Giant</td>
      <td>2019-07-25</td>
      <td>19</td>
      <td>https://open.spotify.com/track/3sEcJ4mGZ9srlXd...</td>
    </tr>
    <tr>
      <th>11</th>
      <td>36bNKiiUjxUCaAO7QtUVfi</td>
      <td>KU LO SA - A COLORS SHOW</td>
      <td>2022-06-10</td>
      <td>1</td>
      <td>https://open.spotify.com/track/2WigMwGJysIh9fR...</td>
    </tr>
    <tr>
      <th>12</th>
      <td>17HtAdJO3qQzLJDf9GAePl</td>
      <td>King Of Love</td>
      <td>2020-06-25</td>
      <td>17</td>
      <td>https://open.spotify.com/track/6nnZHjSHt0ZNtx4...</td>
    </tr>
    <tr>
      <th>13</th>
      <td>3Nt7p3GrkB4QeT1AKONY8U</td>
      <td>Move</td>
      <td>2021-10-13</td>
      <td>1</td>
      <td>https://open.spotify.com/track/6g8Ztyoym7VNLEz...</td>
    </tr>
    <tr>
      <th>14</th>
      <td>0nayxjaX54Frd7GsZq6Pbs</td>
      <td>Rave &amp; Roses Ultra</td>
      <td>2023-04-27</td>
      <td>22</td>
      <td>https://open.spotify.com/track/1iBWjQ9af9NnUd5...</td>
    </tr>
    <tr>
      <th>15</th>
      <td>6blB91ubI6Ul0TFz6X2Non</td>
      <td>Shabba Madda Pot - Single</td>
      <td>2015-05-12</td>
      <td>1</td>
      <td>https://open.spotify.com/track/6S9QZ8QTN5oOUCh...</td>
    </tr>
    <tr>
      <th>16</th>
      <td>34vlTd4355ddD4q9pPsoqF</td>
      <td>African Giant</td>
      <td>2019-07-25</td>
      <td>19</td>
      <td>https://open.spotify.com/track/3a7ziOOO3Cbuv6B...</td>
    </tr>
    <tr>
      <th>17</th>
      <td>6Ds8n0PlFxomLOtEHFwBeo</td>
      <td>No Love</td>
      <td>2023-01-20</td>
      <td>16</td>
      <td>https://open.spotify.com/track/0TTOsyDKykWhCh3...</td>
    </tr>
    <tr>
      <th>18</th>
      <td>2gbx0YcLDduf3oqujoq1fI</td>
      <td>Maverick</td>
      <td>2023-07-27</td>
      <td>20</td>
      <td>https://open.spotify.com/track/3nT2nrfb3FMLg03...</td>
    </tr>
    <tr>
      <th>19</th>
      <td>6lI21W76LD0S3vC55GrfSS</td>
      <td>Timeless</td>
      <td>2023-03-30</td>
      <td>17</td>
      <td>https://open.spotify.com/track/2kaH2Z8ezDUKf6f...</td>
    </tr>
    <tr>
      <th>20</th>
      <td>5wyDRKWKtPq3znLWVOtUIk</td>
      <td>Blessed</td>
      <td>2023-12-01</td>
      <td>18</td>
      <td>https://open.spotify.com/track/3ibXZkzvCPZ6lWb...</td>
    </tr>
    <tr>
      <th>21</th>
      <td>1oSN6MKvpXR5WOHnsPi05w</td>
      <td>Outlaw</td>
      <td>2022-05-06</td>
      <td>7</td>
      <td>https://open.spotify.com/track/1OGZU2zmK6x0UnM...</td>
    </tr>
    <tr>
      <th>22</th>
      <td>0lzPMIAYhhUSD2BPT0VQWI</td>
      <td>Mr. Money With The Vibe</td>
      <td>2022-09-07</td>
      <td>12</td>
      <td>https://open.spotify.com/track/4k4pdUWX8632g7y...</td>
    </tr>
    <tr>
      <th>23</th>
      <td>26du6obYLeY1vf6xIJ1l0D</td>
      <td>Outside</td>
      <td>2018-01-26</td>
      <td>12</td>
      <td>https://open.spotify.com/track/73e0LixjWj3e8pr...</td>
    </tr>
    <tr>
      <th>24</th>
      <td>0uk18xBtNopYpvMT1t7BCU</td>
      <td>Barnabas</td>
      <td>2021-11-18</td>
      <td>7</td>
      <td>https://open.spotify.com/track/03DxO8kGNrEGr1V...</td>
    </tr>
    <tr>
      <th>25</th>
      <td>676QN3uS7pzWA0Or87JTcN</td>
      <td>RU The World</td>
      <td>2023-09-01</td>
      <td>17</td>
      <td>https://open.spotify.com/track/6z5y2kdxF4XrEVR...</td>
    </tr>
    <tr>
      <th>26</th>
      <td>0ZdiHNx2h4QTKwfF7fEM8j</td>
      <td>Realms</td>
      <td>2020-09-10</td>
      <td>7</td>
      <td>https://open.spotify.com/track/6qk3jI8bKCgURI3...</td>
    </tr>
    <tr>
      <th>27</th>
      <td>2e7UIUu34tdxKVkcTG3463</td>
      <td>L.I.T.A</td>
      <td>2023-06-02</td>
      <td>15</td>
      <td>https://open.spotify.com/track/2HfK1KumDffDWPZ...</td>
    </tr>
    <tr>
      <th>28</th>
      <td>7mnGUuvsSbUHZdKkJYdmOg</td>
      <td>The Villain I Never Was</td>
      <td>2022-10-05</td>
      <td>14</td>
      <td>https://open.spotify.com/track/2LqvzGaZniHiZ9C...</td>
    </tr>
    <tr>
      <th>29</th>
      <td>34vlTd4355ddD4q9pPsoqF</td>
      <td>African Giant</td>
      <td>2019-07-25</td>
      <td>19</td>
      <td>https://open.spotify.com/track/7rpWDu9GPlLxbLo...</td>
    </tr>
    <tr>
      <th>30</th>
      <td>1oSN6MKvpXR5WOHnsPi05w</td>
      <td>Outlaw</td>
      <td>2022-05-06</td>
      <td>7</td>
      <td>https://open.spotify.com/track/3IQT2MM49GkXfHF...</td>
    </tr>
    <tr>
      <th>31</th>
      <td>2gbx0YcLDduf3oqujoq1fI</td>
      <td>Maverick</td>
      <td>2023-07-27</td>
      <td>20</td>
      <td>https://open.spotify.com/track/36tVdsRWDbPBekx...</td>
    </tr>
    <tr>
      <th>32</th>
      <td>2O9VJaLSnwjZ2HPpMaVoPU</td>
      <td>Work Of Art</td>
      <td>2023-06-15</td>
      <td>14</td>
      <td>https://open.spotify.com/track/1YgIvHDTvi1vosi...</td>
    </tr>
    <tr>
      <th>33</th>
      <td>2FA3MmXyGWjL0IhoCdktU1</td>
      <td>Anchor Baby</td>
      <td>2021-06-18</td>
      <td>13</td>
      <td>https://open.spotify.com/track/10U0rbctNl1DWEu...</td>
    </tr>
    <tr>
      <th>34</th>
      <td>7mnGUuvsSbUHZdKkJYdmOg</td>
      <td>The Villain I Never Was</td>
      <td>2022-10-05</td>
      <td>14</td>
      <td>https://open.spotify.com/track/3F6xtKBO2YixpP8...</td>
    </tr>
    <tr>
      <th>35</th>
      <td>1JzjwUKkPsdHg1SQ7qa5hc</td>
      <td>I Told Them...</td>
      <td>2023-08-24</td>
      <td>15</td>
      <td>https://open.spotify.com/track/1WsIk6g7dD8LZou...</td>
    </tr>
    <tr>
      <th>36</th>
      <td>5m2xRmSB1D30YZHDHr8556</td>
      <td>Us Against the World</td>
      <td>2022-11-10</td>
      <td>1</td>
      <td>https://open.spotify.com/track/4TaS4giQQK01vKz...</td>
    </tr>
    <tr>
      <th>37</th>
      <td>17HtAdJO3qQzLJDf9GAePl</td>
      <td>King Of Love</td>
      <td>2020-06-25</td>
      <td>17</td>
      <td>https://open.spotify.com/track/1PJUwqQNNWerJeV...</td>
    </tr>
    <tr>
      <th>38</th>
      <td>2iz7b9HLy5aQ81tsMyedNn</td>
      <td>Meridian &amp; Special</td>
      <td>2023-08-25</td>
      <td>2</td>
      <td>https://open.spotify.com/track/09FcXaLu1BdrRNg...</td>
    </tr>
    <tr>
      <th>39</th>
      <td>1uPEctEKBVjCRO5iGsya3b</td>
      <td>Fleur froide - Second état : la cristallisation</td>
      <td>2021-11-19</td>
      <td>41</td>
      <td>https://open.spotify.com/track/1ZrkOlKJ9db1cHn...</td>
    </tr>
    <tr>
      <th>40</th>
      <td>7mnGUuvsSbUHZdKkJYdmOg</td>
      <td>The Villain I Never Was</td>
      <td>2022-10-05</td>
      <td>14</td>
      <td>https://open.spotify.com/track/4DdaGKeVkjQbPHz...</td>
    </tr>
    <tr>
      <th>41</th>
      <td>1JzjwUKkPsdHg1SQ7qa5hc</td>
      <td>I Told Them...</td>
      <td>2023-08-24</td>
      <td>15</td>
      <td>https://open.spotify.com/track/3A17uQFJab0NDpy...</td>
    </tr>
    <tr>
      <th>42</th>
      <td>766bxryPZBL0hjz0KM6VUD</td>
      <td>Beautiful And Brutal Yard</td>
      <td>2023-07-14</td>
      <td>19</td>
      <td>https://open.spotify.com/track/6kgaI3kHkqmRime...</td>
    </tr>
    <tr>
      <th>43</th>
      <td>0uk18xBtNopYpvMT1t7BCU</td>
      <td>Barnabas</td>
      <td>2021-11-18</td>
      <td>7</td>
      <td>https://open.spotify.com/track/1DrfpnLvbwndPSc...</td>
    </tr>
    <tr>
      <th>44</th>
      <td>6e1McsPwHgiySHVlpZRhFx</td>
      <td>EZIOKWU</td>
      <td>2023-10-06</td>
      <td>14</td>
      <td>https://open.spotify.com/track/0QdQh3umB7stVOE...</td>
    </tr>
    <tr>
      <th>45</th>
      <td>4l8Gg5qk0QodyJ12SNtdUf</td>
      <td>Rema</td>
      <td>2019-03-22</td>
      <td>4</td>
      <td>https://open.spotify.com/track/0SjQBdIddPvKSWx...</td>
    </tr>
    <tr>
      <th>46</th>
      <td>34UcYlaPC0yAo0FZV6xoHD</td>
      <td>Bella</td>
      <td>2022-07-08</td>
      <td>1</td>
      <td>https://open.spotify.com/track/0FnoxHCkfmjr2kB...</td>
    </tr>
    <tr>
      <th>47</th>
      <td>34vlTd4355ddD4q9pPsoqF</td>
      <td>African Giant</td>
      <td>2019-07-25</td>
      <td>19</td>
      <td>https://open.spotify.com/track/1PoJXULCvl03b1f...</td>
    </tr>
    <tr>
      <th>48</th>
      <td>3WlxlO16ydHEisWjriRpHk</td>
      <td>Butta My Bread</td>
      <td>2023-04-07</td>
      <td>1</td>
      <td>https://open.spotify.com/track/3aJF7HsFOwuUAFO...</td>
    </tr>
    <tr>
      <th>49</th>
      <td>2gbx0YcLDduf3oqujoq1fI</td>
      <td>Maverick</td>
      <td>2023-07-27</td>
      <td>20</td>
      <td>https://open.spotify.com/track/5a8IYhZWozHBb0b...</td>
    </tr>
  </tbody>
</table>
</div>




```python
album_df['album_release_date'] = pd.to_datetime(album_df['album_release_date'])
```


```python
album_df.info()
```

    <class 'pandas.core.frame.DataFrame'>
    RangeIndex: 50 entries, 0 to 49
    Data columns (total 5 columns):
     #   Column               Non-Null Count  Dtype         
    ---  ------               --------------  -----         
     0   album_id             50 non-null     object        
     1   album_name           50 non-null     object        
     2   album_release_date   50 non-null     datetime64[ns]
     3   album_total_tracks   50 non-null     int64         
     4   album_external_urls  50 non-null     object        
    dtypes: datetime64[ns](1), int64(1), object(3)
    memory usage: 2.1+ KB
    


```python
song_df
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>song_id</th>
      <th>song_name</th>
      <th>duration_ms</th>
      <th>song_url</th>
      <th>popularity</th>
      <th>song_added</th>
      <th>album_id</th>
      <th>artist_id</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>4RoKNqyZ9622tcAeNPNv5k</td>
      <td>City Boys</td>
      <td>153346</td>
      <td>https://open.spotify.com/track/4RoKNqyZ9622tcA...</td>
      <td>81</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>1JzjwUKkPsdHg1SQ7qa5hc</td>
      <td>3wcj11K77LjEY1PkEazffa</td>
    </tr>
    <tr>
      <th>1</th>
      <td>5aIVCx5tnk0ntmdiinnYvw</td>
      <td>Water</td>
      <td>200255</td>
      <td>https://open.spotify.com/track/5aIVCx5tnk0ntmd...</td>
      <td>94</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>22sXXkKgjEuawIFL1e1tRw</td>
      <td>3SozjO3Lat463tQICI9LcE</td>
    </tr>
    <tr>
      <th>2</th>
      <td>6TTR7tXftck5lU7BPRY7bV</td>
      <td>Santorini Coffee</td>
      <td>134365</td>
      <td>https://open.spotify.com/track/6TTR7tXftck5lU7...</td>
      <td>71</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>4np0ohQb06VAAitOpk3Rt4</td>
      <td>4Xj0nxVO4r7PLEaw7LRiBa</td>
    </tr>
    <tr>
      <th>3</th>
      <td>1eldTykrnkEBLX41bk5eMw</td>
      <td>Petit génie</td>
      <td>217259</td>
      <td>https://open.spotify.com/track/1eldTykrnkEBLX4...</td>
      <td>80</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>4Ta3fRzeMUtQlQrrcn1cuE</td>
      <td>6L8y2rKomt32RmT4wfwZS7</td>
    </tr>
    <tr>
      <th>4</th>
      <td>2FDTHlrBguDzQkp7PVj16Q</td>
      <td>Sprinter</td>
      <td>229133</td>
      <td>https://open.spotify.com/track/2FDTHlrBguDzQkp...</td>
      <td>89</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>5l0QlaI3wdZpE7ggoO5Rwg</td>
      <td>6Ip8FS7vWT1uKkJSweANQK</td>
    </tr>
    <tr>
      <th>5</th>
      <td>5YbPxJwPfrj7uswNwoF1pJ</td>
      <td>Last Last</td>
      <td>172342</td>
      <td>https://open.spotify.com/track/5YbPxJwPfrj7usw...</td>
      <td>79</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>6kgDkAupBVRSqbJPUaTJwQ</td>
      <td>3wcj11K77LjEY1PkEazffa</td>
    </tr>
    <tr>
      <th>6</th>
      <td>0TZMDJP2MrGTSmWqUnswUh</td>
      <td>Shu-Peru</td>
      <td>139377</td>
      <td>https://open.spotify.com/track/0TZMDJP2MrGTSmW...</td>
      <td>63</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>2gbx0YcLDduf3oqujoq1fI</td>
      <td>1X6cBGnXpEpN7CmflLKmLV</td>
    </tr>
    <tr>
      <th>7</th>
      <td>6BWgLorAwF17ofyu8361HM</td>
      <td>Cast</td>
      <td>129123</td>
      <td>https://open.spotify.com/track/6BWgLorAwF17ofy...</td>
      <td>72</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>14VJEhvxRCOsNtcwjjBxwR</td>
      <td>4TKhxSkqClXrdtUWgKqHVU</td>
    </tr>
    <tr>
      <th>8</th>
      <td>1wADwLSkYhrSmy4vdy6BRn</td>
      <td>soso</td>
      <td>183056</td>
      <td>https://open.spotify.com/track/1wADwLSkYhrSmy4...</td>
      <td>76</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>5NLjxx8nRy9ooUmgpOvfem</td>
      <td>5yOvAmpIR7hVxiS6Ls5DPO</td>
    </tr>
    <tr>
      <th>9</th>
      <td>30RBuEKVJ2UXimaPtwAEIa</td>
      <td>Sans effet</td>
      <td>160530</td>
      <td>https://open.spotify.com/track/30RBuEKVJ2UXima...</td>
      <td>61</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>1uPEctEKBVjCRO5iGsya3b</td>
      <td>7gU9VyFRN3JWPJ5oHOil60</td>
    </tr>
    <tr>
      <th>10</th>
      <td>3sEcJ4mGZ9srlXdG7G2HK1</td>
      <td>Pull Up</td>
      <td>187866</td>
      <td>https://open.spotify.com/track/3sEcJ4mGZ9srlXd...</td>
      <td>51</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>34vlTd4355ddD4q9pPsoqF</td>
      <td>3wcj11K77LjEY1PkEazffa</td>
    </tr>
    <tr>
      <th>11</th>
      <td>2WigMwGJysIh9fRnSJvpjn</td>
      <td>KU LO SA - A COLORS SHOW</td>
      <td>147580</td>
      <td>https://open.spotify.com/track/2WigMwGJysIh9fR...</td>
      <td>77</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>36bNKiiUjxUCaAO7QtUVfi</td>
      <td>3WTrdbZU99dgTtt3ZkyamT</td>
    </tr>
    <tr>
      <th>12</th>
      <td>6nnZHjSHt0ZNtx4bIUky9P</td>
      <td>Boys Are Bad</td>
      <td>137000</td>
      <td>https://open.spotify.com/track/6nnZHjSHt0ZNtx4...</td>
      <td>64</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>17HtAdJO3qQzLJDf9GAePl</td>
      <td>1X6cBGnXpEpN7CmflLKmLV</td>
    </tr>
    <tr>
      <th>13</th>
      <td>6g8Ztyoym7VNLEzl8alsJK</td>
      <td>Move</td>
      <td>150491</td>
      <td>https://open.spotify.com/track/6g8Ztyoym7VNLEz...</td>
      <td>57</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>3Nt7p3GrkB4QeT1AKONY8U</td>
      <td>68R39izwNAztATrXMOqkJS</td>
    </tr>
    <tr>
      <th>14</th>
      <td>1iBWjQ9af9NnUd5xnQDB3k</td>
      <td>Charm</td>
      <td>204750</td>
      <td>https://open.spotify.com/track/1iBWjQ9af9NnUd5...</td>
      <td>74</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>0nayxjaX54Frd7GsZq6Pbs</td>
      <td>46pWGuE3dSwY3bMMXGBvVS</td>
    </tr>
    <tr>
      <th>15</th>
      <td>6S9QZ8QTN5oOUChcYWChnK</td>
      <td>Shabba Madda Pot</td>
      <td>142978</td>
      <td>https://open.spotify.com/track/6S9QZ8QTN5oOUCh...</td>
      <td>61</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>6blB91ubI6Ul0TFz6X2Non</td>
      <td>28UDeKu2FPrU0T7dpUiSGY</td>
    </tr>
    <tr>
      <th>16</th>
      <td>3a7ziOOO3Cbuv6BMXrj0wU</td>
      <td>Killin Dem (feat. Zlatan)</td>
      <td>221100</td>
      <td>https://open.spotify.com/track/3a7ziOOO3Cbuv6B...</td>
      <td>50</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>34vlTd4355ddD4q9pPsoqF</td>
      <td>3wcj11K77LjEY1PkEazffa</td>
    </tr>
    <tr>
      <th>17</th>
      <td>0TTOsyDKykWhCh3qDd9wMY</td>
      <td>Talibans</td>
      <td>188737</td>
      <td>https://open.spotify.com/track/0TTOsyDKykWhCh3...</td>
      <td>70</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>6Ds8n0PlFxomLOtEHFwBeo</td>
      <td>3IDfJpj4YVkaBl7Dd52Pxv</td>
    </tr>
    <tr>
      <th>18</th>
      <td>3nT2nrfb3FMLg03W4mPaBl</td>
      <td>Cough (Odo)</td>
      <td>176195</td>
      <td>https://open.spotify.com/track/3nT2nrfb3FMLg03...</td>
      <td>68</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>2gbx0YcLDduf3oqujoq1fI</td>
      <td>1X6cBGnXpEpN7CmflLKmLV</td>
    </tr>
    <tr>
      <th>19</th>
      <td>2kaH2Z8ezDUKf6fNw250rZ</td>
      <td>UNAVAILABLE (feat. Musa Keys)</td>
      <td>169911</td>
      <td>https://open.spotify.com/track/2kaH2Z8ezDUKf6f...</td>
      <td>78</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>6lI21W76LD0S3vC55GrfSS</td>
      <td>0Y3agQaa6g2r0YmHPOO9rh</td>
    </tr>
    <tr>
      <th>20</th>
      <td>3ibXZkzvCPZ6lWbfubSolQ</td>
      <td>THIS YEAR (Blessings)</td>
      <td>126206</td>
      <td>https://open.spotify.com/track/3ibXZkzvCPZ6lWb...</td>
      <td>62</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>5wyDRKWKtPq3znLWVOtUIk</td>
      <td>5c0lDrNyT2RnFhujZpPIas</td>
    </tr>
    <tr>
      <th>21</th>
      <td>1OGZU2zmK6x0UnM3yeZ4lR</td>
      <td>Apollo</td>
      <td>170000</td>
      <td>https://open.spotify.com/track/1OGZU2zmK6x0UnM...</td>
      <td>65</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>1oSN6MKvpXR5WOHnsPi05w</td>
      <td>1E5hfn5BduN2nnoZCJmUVG</td>
    </tr>
    <tr>
      <th>22</th>
      <td>4k4pdUWX8632g7yByxC3rS</td>
      <td>Sungba (feat. Burna Boy) - Remix</td>
      <td>210000</td>
      <td>https://open.spotify.com/track/4k4pdUWX8632g7y...</td>
      <td>66</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>0lzPMIAYhhUSD2BPT0VQWI</td>
      <td>3a1tBryiczPAZpgoZN9Rzg</td>
    </tr>
    <tr>
      <th>23</th>
      <td>73e0LixjWj3e8prfptVeGD</td>
      <td>More Life</td>
      <td>92342</td>
      <td>https://open.spotify.com/track/73e0LixjWj3e8pr...</td>
      <td>58</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>26du6obYLeY1vf6xIJ1l0D</td>
      <td>3wcj11K77LjEY1PkEazffa</td>
    </tr>
    <tr>
      <th>24</th>
      <td>03DxO8kGNrEGr1VjPSdQs2</td>
      <td>Lie</td>
      <td>156600</td>
      <td>https://open.spotify.com/track/03DxO8kGNrEGr1V...</td>
      <td>66</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>0uk18xBtNopYpvMT1t7BCU</td>
      <td>1X6cBGnXpEpN7CmflLKmLV</td>
    </tr>
    <tr>
      <th>25</th>
      <td>6z5y2kdxF4XrEVRFVqdGVL</td>
      <td>Asiwaju</td>
      <td>216000</td>
      <td>https://open.spotify.com/track/6z5y2kdxF4XrEVR...</td>
      <td>67</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>676QN3uS7pzWA0Or87JTcN</td>
      <td>0a1SidMjD8D6EHvJph4n2H</td>
    </tr>
    <tr>
      <th>26</th>
      <td>6qk3jI8bKCgURI3h0d8zBZ</td>
      <td>Again</td>
      <td>156083</td>
      <td>https://open.spotify.com/track/6qk3jI8bKCgURI3...</td>
      <td>71</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>0ZdiHNx2h4QTKwfF7fEM8j</td>
      <td>1fYVmAFB7sC7eDoF3mJXla</td>
    </tr>
    <tr>
      <th>27</th>
      <td>2HfK1KumDffDWPZga46Hmw</td>
      <td>Sugarcane</td>
      <td>156781</td>
      <td>https://open.spotify.com/track/2HfK1KumDffDWPZ...</td>
      <td>53</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>2e7UIUu34tdxKVkcTG3463</td>
      <td>6Z9Xe5mjocmPOhz2TLNrAi</td>
    </tr>
    <tr>
      <th>28</th>
      <td>2LqvzGaZniHiZ9CXhzkclD</td>
      <td>Kwaku The Traveller</td>
      <td>185364</td>
      <td>https://open.spotify.com/track/2LqvzGaZniHiZ9C...</td>
      <td>59</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>7mnGUuvsSbUHZdKkJYdmOg</td>
      <td>2LiqbH7OhqP0yuaG8VL1wJ</td>
    </tr>
    <tr>
      <th>29</th>
      <td>7rpWDu9GPlLxbLorYKVys7</td>
      <td>Gbona</td>
      <td>187609</td>
      <td>https://open.spotify.com/track/7rpWDu9GPlLxbLo...</td>
      <td>70</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>34vlTd4355ddD4q9pPsoqF</td>
      <td>3wcj11K77LjEY1PkEazffa</td>
    </tr>
    <tr>
      <th>30</th>
      <td>3IQT2MM49GkXfHF9eemaw5</td>
      <td>Soweto</td>
      <td>148000</td>
      <td>https://open.spotify.com/track/3IQT2MM49GkXfHF...</td>
      <td>75</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>1oSN6MKvpXR5WOHnsPi05w</td>
      <td>1E5hfn5BduN2nnoZCJmUVG</td>
    </tr>
    <tr>
      <th>31</th>
      <td>36tVdsRWDbPBekxVYEWhph</td>
      <td>Buga (Lo Lo Lo)</td>
      <td>183103</td>
      <td>https://open.spotify.com/track/36tVdsRWDbPBekx...</td>
      <td>63</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>2gbx0YcLDduf3oqujoq1fI</td>
      <td>1X6cBGnXpEpN7CmflLKmLV</td>
    </tr>
    <tr>
      <th>32</th>
      <td>1YgIvHDTvi1vosins1jyAC</td>
      <td>Amapiano</td>
      <td>165000</td>
      <td>https://open.spotify.com/track/1YgIvHDTvi1vosi...</td>
      <td>70</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>2O9VJaLSnwjZ2HPpMaVoPU</td>
      <td>3a1tBryiczPAZpgoZN9Rzg</td>
    </tr>
    <tr>
      <th>33</th>
      <td>10U0rbctNl1DWEuCn1ETm6</td>
      <td>𝘠𝘚𝘓</td>
      <td>173714</td>
      <td>https://open.spotify.com/track/10U0rbctNl1DWEu...</td>
      <td>63</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>2FA3MmXyGWjL0IhoCdktU1</td>
      <td>7dYb5EKtRnRaWM0GQ12cKC</td>
    </tr>
    <tr>
      <th>34</th>
      <td>3F6xtKBO2YixpP8lFJTiGo</td>
      <td>Konongo Zongo</td>
      <td>161699</td>
      <td>https://open.spotify.com/track/3F6xtKBO2YixpP8...</td>
      <td>59</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>7mnGUuvsSbUHZdKkJYdmOg</td>
      <td>2LiqbH7OhqP0yuaG8VL1wJ</td>
    </tr>
    <tr>
      <th>35</th>
      <td>1WsIk6g7dD8LZouywnzGUb</td>
      <td>Talibans II - Bonus Track</td>
      <td>176453</td>
      <td>https://open.spotify.com/track/1WsIk6g7dD8LZou...</td>
      <td>67</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>1JzjwUKkPsdHg1SQ7qa5hc</td>
      <td>3wcj11K77LjEY1PkEazffa</td>
    </tr>
    <tr>
      <th>36</th>
      <td>4TaS4giQQK01vKzBB40AEY</td>
      <td>Us Against the World</td>
      <td>139786</td>
      <td>https://open.spotify.com/track/4TaS4giQQK01vKz...</td>
      <td>72</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>5m2xRmSB1D30YZHDHr8556</td>
      <td>33X2jfLSVyDevoksJjRZoS</td>
    </tr>
    <tr>
      <th>37</th>
      <td>1PJUwqQNNWerJeVYFm1GEO</td>
      <td>We Wan Comot</td>
      <td>124868</td>
      <td>https://open.spotify.com/track/1PJUwqQNNWerJeV...</td>
      <td>62</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>17HtAdJO3qQzLJDf9GAePl</td>
      <td>1X6cBGnXpEpN7CmflLKmLV</td>
    </tr>
    <tr>
      <th>38</th>
      <td>09FcXaLu1BdrRNgxyBi6p5</td>
      <td>Meridian</td>
      <td>255160</td>
      <td>https://open.spotify.com/track/09FcXaLu1BdrRNg...</td>
      <td>78</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>2iz7b9HLy5aQ81tsMyedNn</td>
      <td>6Ip8FS7vWT1uKkJSweANQK</td>
    </tr>
    <tr>
      <th>39</th>
      <td>1ZrkOlKJ9db1cHnL1xEyfd</td>
      <td>P A S C O M M E Ç A</td>
      <td>178226</td>
      <td>https://open.spotify.com/track/1ZrkOlKJ9db1cHn...</td>
      <td>69</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>1uPEctEKBVjCRO5iGsya3b</td>
      <td>7gU9VyFRN3JWPJ5oHOil60</td>
    </tr>
    <tr>
      <th>40</th>
      <td>4DdaGKeVkjQbPHzpoHGafk</td>
      <td>Second Sermon - Remix</td>
      <td>194863</td>
      <td>https://open.spotify.com/track/4DdaGKeVkjQbPHz...</td>
      <td>59</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>7mnGUuvsSbUHZdKkJYdmOg</td>
      <td>2LiqbH7OhqP0yuaG8VL1wJ</td>
    </tr>
    <tr>
      <th>41</th>
      <td>3A17uQFJab0NDpyIeZAavF</td>
      <td>Big 7</td>
      <td>143042</td>
      <td>https://open.spotify.com/track/3A17uQFJab0NDpy...</td>
      <td>67</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>1JzjwUKkPsdHg1SQ7qa5hc</td>
      <td>3wcj11K77LjEY1PkEazffa</td>
    </tr>
    <tr>
      <th>42</th>
      <td>6kgaI3kHkqmRimeGQdS4Ga</td>
      <td>Who Told You (feat. Drake)</td>
      <td>208920</td>
      <td>https://open.spotify.com/track/6kgaI3kHkqmRime...</td>
      <td>70</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>766bxryPZBL0hjz0KM6VUD</td>
      <td>2a0uxJgbvvIRI4GX8pYfcr</td>
    </tr>
    <tr>
      <th>43</th>
      <td>1DrfpnLvbwndPScRLwbUE0</td>
      <td>Pour Me Water</td>
      <td>146399</td>
      <td>https://open.spotify.com/track/1DrfpnLvbwndPSc...</td>
      <td>64</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>0uk18xBtNopYpvMT1t7BCU</td>
      <td>1X6cBGnXpEpN7CmflLKmLV</td>
    </tr>
    <tr>
      <th>44</th>
      <td>0QdQh3umB7stVOExuHlWvl</td>
      <td>DECLAN RICE</td>
      <td>124000</td>
      <td>https://open.spotify.com/track/0QdQh3umB7stVOE...</td>
      <td>64</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>6e1McsPwHgiySHVlpZRhFx</td>
      <td>3LOm0AZjpwVQebvkyanjDy</td>
    </tr>
    <tr>
      <th>45</th>
      <td>0SjQBdIddPvKSWxr8vk6QX</td>
      <td>Dumebi</td>
      <td>179775</td>
      <td>https://open.spotify.com/track/0SjQBdIddPvKSWx...</td>
      <td>67</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>4l8Gg5qk0QodyJ12SNtdUf</td>
      <td>46pWGuE3dSwY3bMMXGBvVS</td>
    </tr>
    <tr>
      <th>46</th>
      <td>0FnoxHCkfmjr2kBDwos4OG</td>
      <td>Bella</td>
      <td>146478</td>
      <td>https://open.spotify.com/track/0FnoxHCkfmjr2kB...</td>
      <td>54</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>34UcYlaPC0yAo0FZV6xoHD</td>
      <td>2TwUVWFJs4LD0lOBbJXnNa</td>
    </tr>
    <tr>
      <th>47</th>
      <td>1PoJXULCvl03b1fiZmMxmd</td>
      <td>On the Low</td>
      <td>185898</td>
      <td>https://open.spotify.com/track/1PoJXULCvl03b1f...</td>
      <td>73</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>34vlTd4355ddD4q9pPsoqF</td>
      <td>3wcj11K77LjEY1PkEazffa</td>
    </tr>
    <tr>
      <th>48</th>
      <td>3aJF7HsFOwuUAFOaRMQCxR</td>
      <td>Butta My Bread</td>
      <td>148672</td>
      <td>https://open.spotify.com/track/3aJF7HsFOwuUAFO...</td>
      <td>72</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>3WlxlO16ydHEisWjriRpHk</td>
      <td>3gYUwwn7FiiBMKHe36OUaQ</td>
    </tr>
    <tr>
      <th>49</th>
      <td>5a8IYhZWozHBb0bmqbogyq</td>
      <td>RTID (Rich Till I Die)</td>
      <td>172944</td>
      <td>https://open.spotify.com/track/5a8IYhZWozHBb0b...</td>
      <td>59</td>
      <td>1970-01-01T00:00:00Z</td>
      <td>2gbx0YcLDduf3oqujoq1fI</td>
      <td>1X6cBGnXpEpN7CmflLKmLV</td>
    </tr>
  </tbody>
</table>
</div>




```python
song_df['song_added'] = pd.to_datetime(song_df['song_added']) 
```


```python
song_df.info()
```

    <class 'pandas.core.frame.DataFrame'>
    RangeIndex: 50 entries, 0 to 49
    Data columns (total 8 columns):
     #   Column       Non-Null Count  Dtype              
    ---  ------       --------------  -----              
     0   song_id      50 non-null     object             
     1   song_name    50 non-null     object             
     2   duration_ms  50 non-null     int64              
     3   song_url     50 non-null     object             
     4   popularity   50 non-null     int64              
     5   song_added   50 non-null     datetime64[ns, UTC]
     6   album_id     50 non-null     object             
     7   artist_id    50 non-null     object             
    dtypes: datetime64[ns, UTC](1), int64(2), object(5)
    memory usage: 3.3+ KB
    


```python
song_df.head()
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>song_id</th>
      <th>song_name</th>
      <th>duration_ms</th>
      <th>song_url</th>
      <th>popularity</th>
      <th>song_added</th>
      <th>album_id</th>
      <th>artist_id</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>4RoKNqyZ9622tcAeNPNv5k</td>
      <td>City Boys</td>
      <td>153346</td>
      <td>https://open.spotify.com/track/4RoKNqyZ9622tcA...</td>
      <td>81</td>
      <td>1970-01-01 00:00:00+00:00</td>
      <td>1JzjwUKkPsdHg1SQ7qa5hc</td>
      <td>3wcj11K77LjEY1PkEazffa</td>
    </tr>
    <tr>
      <th>1</th>
      <td>5aIVCx5tnk0ntmdiinnYvw</td>
      <td>Water</td>
      <td>200255</td>
      <td>https://open.spotify.com/track/5aIVCx5tnk0ntmd...</td>
      <td>94</td>
      <td>1970-01-01 00:00:00+00:00</td>
      <td>22sXXkKgjEuawIFL1e1tRw</td>
      <td>3SozjO3Lat463tQICI9LcE</td>
    </tr>
    <tr>
      <th>2</th>
      <td>6TTR7tXftck5lU7BPRY7bV</td>
      <td>Santorini Coffee</td>
      <td>134365</td>
      <td>https://open.spotify.com/track/6TTR7tXftck5lU7...</td>
      <td>71</td>
      <td>1970-01-01 00:00:00+00:00</td>
      <td>4np0ohQb06VAAitOpk3Rt4</td>
      <td>4Xj0nxVO4r7PLEaw7LRiBa</td>
    </tr>
    <tr>
      <th>3</th>
      <td>1eldTykrnkEBLX41bk5eMw</td>
      <td>Petit génie</td>
      <td>217259</td>
      <td>https://open.spotify.com/track/1eldTykrnkEBLX4...</td>
      <td>80</td>
      <td>1970-01-01 00:00:00+00:00</td>
      <td>4Ta3fRzeMUtQlQrrcn1cuE</td>
      <td>6L8y2rKomt32RmT4wfwZS7</td>
    </tr>
    <tr>
      <th>4</th>
      <td>2FDTHlrBguDzQkp7PVj16Q</td>
      <td>Sprinter</td>
      <td>229133</td>
      <td>https://open.spotify.com/track/2FDTHlrBguDzQkp...</td>
      <td>89</td>
      <td>1970-01-01 00:00:00+00:00</td>
      <td>5l0QlaI3wdZpE7ggoO5Rwg</td>
      <td>6Ip8FS7vWT1uKkJSweANQK</td>
    </tr>
  </tbody>
</table>
</div>




```python

```


```python

```


```python

```
