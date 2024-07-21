### 2024-07-21

Long-shot project idea. I/we could collect recordings from [ParlVu](https://parlvu.parl.gc.ca/Harmony/en/View/UpcomingEvents). [Terms of service](https://www.ourcommons.ca/Content/Misc/parlvu-faq-e.pdf) permit non-commercial use, notwithstanding reports to Standing Committees that may have their own copyright issues. There are I'd guess thousands of hours of video and audio. Some recordings are audio only, and not all have closed captions but some do. I'd guess these are the motherlode: created by professional stenographers in both languages.

They have a download tool that gives a direct link to an mp3/4, which is great for debugging. But these file types don't include the closed captions (AFAIK). When you play a video in the browser, CC or not, you get `.ts` files of type MP2T. If you just curl any of those requests and play it in VLC, you do see the CC. Presumably, you could use FFMPEG to also extract the subtitles as plain text.

Downloading content this way would require streaming them in real time. The download tool would speed things up in cases where no subtitles can be downloaded anyways. And we'd want to create an index of all the content to get an idea of how much is video vs audio, what has subtitles, and how long everything is. Storage could be more than a terabyte? I have no idea. 

Due to these long runtimes and likely huge storage requirements, this would be difficult as a personal project.

### 2024-07-21

Turns out all this data already exists in transcript form, at least at the committee level. Search first next time.