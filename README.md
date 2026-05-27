# youtube_downloader

from pytube import YouTube

url = input("لینک ویدیو: ")
yt = YouTube(url)
stream = yt.streams.get_highest_resolution()
stream.download()
