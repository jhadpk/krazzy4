# krazzy4
Project for Spark - Design+Hack-athon


##Java API(s)

>curl -v http://localhost:9099/Spark/api/getImagesFiles -d '/Users/yogeesh.rajendra/Desktop/test.html$/Users/yogeesh.rajendra/Desktop/test1.html$/Users/yogeesh.rajendra/Desktop/test2.html' -H 'Content-Type: application/json'

`To start server : ./restartserver.sh`


curl -v http://localhost:9099/Spark/api/getPOST -d '/Users/yogeesh.rajendra/Desktop/test.html$/Users/yogeesh.rajendra/Desktop/test1.html$/Users/yogeesh.rajendra/Desktop/test2.html' -H 'Content-Type: application/json'

curl http://localhost:9099/Spark/api/getVideoFiles -d 'TESTCampaign$/Users/yogeesh.rajendra/Desktop/fk.mp3$/Users/yogeesh.rajendra/Desktop/margin.html^33$/Users/yogeesh.rajendra/Desktop/test1.html^33$/Users/yogeesh.rajendra/Desktop/test2.html^33#TESTCampaign1$/Users/yogeesh.rajendra/Desktop/fk.mp3$/Users/yogeesh.rajendra/Desktop/margin.html^33$/Users/yogeesh.rajendra/Desktop/test1.html^33$/Users/yogeesh.rajendra/Desktop/test2.html^33' -H 'Content-Type: application/json'

ffmpeg -r 1/5 -i /Users/yogeesh.rajendra/Documents/HUB/Personal/work/github/krazzy4/src/main/resources/TESTCampaign1.txt -c:v libx264 -vf fps=25 -pix_fmt yuv420p /opt/spark/dump/TESTCampaign/videos/out.mp4



ffmpeg -r 60 -f image2 -s 1920x1080 -i /opt/spark/dump/TESTCampaign/images/pic%01d.jpg -vcodec libx264 -crf 25  -pix_fmt yuv420p /opt/spark/dump/TESTCampaign/videos/out.mp4


ffmpeg -i /opt/spark/dump/TESTCampaign/images/pic%01d.jpg /tmp/out.mpg

ffmpeg -ss 00:23:00 -i /opt/spark/dump/TESTCampaign/images/pic%01d.jpg /tmp/out.mp4