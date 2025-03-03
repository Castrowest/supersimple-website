import yt_dlp

def download_music(url, output_path="downloads/%(title)s.%(ext)s"):
    options = {
        'format': 'bestaudio/best',
        'postprocessors': [{
            'key': 'FFmpegExtractAudio',
            'preferredcodec': 'mp3',
            'preferredquality': '192',
        }],
        'outtmpl': output_path,
    }
    
    with yt_dlp.YoutubeDL(options) as ydl:
        ydl.download([uhttps://www.youtube.com/redirect?event=video_description&redir_token=QUFFLUhqbTU5NVhrZmh3MWx3WHFvOVo4RVBlNmlrUWR0d3xBQ3Jtc0tsTi0zRzBxcFlMamhNNWszaFQyTUhtT1lTSS1YSzdvWmd5SmRPTHk1ajcwVDF5OGRCMkxKa1c2NU10eDkydXhacUpXR01ZRExvdC1RU0x3YnJCcndONVFWNmRJbjdTUktiYWtyeTc5NlotUFlVWW1rVQ&q=https%3A%2F%2Fdavido.lnk.to%2Ftimeless&v=OSBan_sH_b8rl])

if __name__ == "__main__":
    url = input("Enterhttps://www.google.com/search?sca_esv=cd82cf180911c650&cs=0&sxsrf=AHTn8zpaD0l1Suqb6cRhPCct7qaqZrL8FQ:1740974965658&q=davido+assurance&stick=H4sIAAAAAAAAAONgFuLSz9U3iDfMyjYxVeLVT9c3NEwzLTSrLLM01xL0LS3OTHYsKsksLgnJD87PS1_EKpCSWJaZkq-QWFxcWpSYl5wKAGPhkJ5DAAAA&sa=X&ved=2ahUKEwiN1o6The2LAxWa_7sIHQQrEh8Qri56BAgLEAM the music URL: ")
    download_music(url)
    print("Download complete!") 
