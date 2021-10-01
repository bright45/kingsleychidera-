# kingsleychidera-
Speaker 1 (00:00):
One of the most useful tools you have for supporting and managing the nomad service is InControl 2.
New Speaker (00:06):
Incontrol 2 gives you full visibility and remote support capability of any of these devices, wherever they're deployed.
New Speaker (00:16):
What I'm going to show you today is the screens and areas within InControl 2 that are likely going to be most useful to you on a day-to-day basis.
New Speaker (00:25):
So let's, let's jump in and have a look.
New Speaker (00:28):
Right now, this is a training group set up for this video. So at the moment, there are only two devices in this group. When you login into InControl 2, you'll have visibility of those devices that you're looking to support, but even here, even with just two devices, as a couple of things, I can, I can show you one of those is, if you imagine this was a long list and I was looking in particular for my device, I can do a live interactive filter here, search for a name or a serial number, and filter all of the devices in this group by that that string, all that content.
Speaker 1 (01:06):
And so here's, Martin's nomad - that is mine over there on the workbench, and at a glance here, I can see that it's currently online, cause it status is green. I can see which product it is. I can see how long it's been turned on and how long it's been connected to the internet. And at what time it was, it was turned on. I can see that it's currently connected via cellular one and two because they're both green and they're both visible there. And if I hover over those, I can see all the details about that particular Cellular connection. I can see the signal strength. I can see the IP addressing. I can see the ICCID and the IMSI, all of that sort of information is there.
New Speaker (01:48):
Moving on to the right, I can see live usage information. This is live bandwidth. And to the right of that, the number of clients that are actively using or connected and using the, the bandwidth through the router.
New Speaker (02:02):
Now clients is interesting. That is the number of IP addresses that are currently talking through the nomad service. So if nomad is acting as the firewall and the primary gateway, and you've got a bunch of laptops and PCs and, and whatever, hanging off the back of it, then we'll see a number count here for all of those devices that are talking through nomad. However, if there is a customer firewall and then behind that, we've got all of the customer appliances and laptops and devices then the only IP address we get to see is the firewall IP. So don't be surprised if sometimes the clients listed is just one and other times it could be a hundred or more, and we can see the firmware level there as well. And also to the right, when the last configuration was applied which is useful if a customer up and says, oh, it's working great. Oh, it's not working today, but it is working great yesterday. And then you can see that there's been changes applied and go and investigate what those changes might have been.
New Speaker (03:11):
So let's click through and go and look at the detail for this device.
Speaker 1 (03:17):
So in the device details screen, we get to see a little bit more detail. Of course we get to see the and we can click through into things like the event log. We can do show all here and see the serial number and the information about individual modems on the device. We can get the local username, admin passwords. We can log in locally too, if we need to. And things like that.
New Speaker (03:46):
We've also got configuration backups. So whenever a configuration changes that configuration is stored here in, in control two, which means we can download and restore configurations. If we ever make a mistake, or if we need to swap out a device, one for another, in this custom configuration, we can download the configuration from the original device and upload it to the new one, which is kind of handy.
New Speaker (04:13):
On the right, We've got visibility of all of the current active Wan connections of which there's two at the moment. These are both connected to three UK cause I'm in the UK and we can see that there are on LTE and they are roaming, and we can see,ucurrent signal levels as well. Just like before, if we click on details, we can see more detail. And here we get more information about signal strength and quality and RSRQ is one of the best indicators as to the quality of connection. Of course. Uyeah.
Speaker 1 (04:50):
Now from a day-to-day perspective, you are going to want to know a number of things. When a customer calls up about a nomad device, one of those things is definitely how is it connected at the moment? Is it online? Does it look happy?
New Speaker (05:04):
Well this is a happy looking device. Both the cellular WANS are connected and we've got a connected client there and data is being used, not a huge amount, but some data is definitely being used there.
New Speaker (05:19):
What we can do now is it's just get the device over there. I've got a laptop plugged into the nomad. And what we're going to do is get that to consume a bit more data so we can see in real time what happens. I'm going to grab across a remote desktop session...
New Speaker (05:38):
... And let's stream some video from the connected laptop so we can actually see in real time how the InControl2 updates us about the current bandwidth usage.
Speaker 1 (05:51):
So there we are, we're streaming a video on YouTube. Let me just get this out of the way for now. And immediately we can see usage is changing here in real time, and what we've also got up here, if we do bandwidth and usage reports, is we can see in real time what bandwidth is being used. And I've already opened this tab actually, before I started the video. So what we can see here is actually this graph that real-time graph has been running for the last 20 minutes or so 10 minutes. And we can see how usage has varied over time. We can also see that there was peak usage, well is peak usage over this period of just under 2Mbps of data.
New Speaker (06:36):
So this is can be really handy, right? If a customer calls up and says the system feels slow today and you come into InControl 2 you have a look at the device, you look at real time bandwidth, and you say, well, hang on a minute.
Speaker 1 (06:50):
There's 20 Mbps of bandwidth being currently used. So the system is doing great. Why what's what we need to look at is which devices are using that bandwidth. Now to do that, I've got a couple of ways.
New Speaker (07:04):
Probably the easiest (or the quickest) is actually to go to remote WebAdmin on the device. And what that does is that creates a tunnel from the device back to InControl 2, and then it gives us a media access to the web interface of that device.
New Speaker (07:20):
And in that view, we can go to status, client list, and we can see a list of connected clients and how much bandwidth they are using.
New Speaker (07:33):
So, you'll be able to tell the customer which device on the network is consuming the most amount of bandwidth.
Speaker 1 (07:41):
Another way to do this is to - if back at the device level, or rather back here looking at the device and InControl 2 we can do device reports.
New Speaker (07:55):
Now this is a test device, so we're not going to - which I've only just turned on. So we're not going to see historic data here yet, but, what you would be able to see on a device that's been up and running with lots of clients connected is a list of those clients, which ones are the heaviest users, and how much data they've used. So you'd be able to see trends in usage and identify perhaps somebody who's streaming too much video or a server that's doing too many OS updates, or that sort of thing.
Speaker 1 (08:31):
The other really useful place on InControl 2, particularly when a customer calls and says that it's worse today than yesterday, or 'it was great two days ago, and now it's not so great what's happened?', is the cellular quality reports or the WAN quality reports. Let's go look at those.
New Speaker (08:52):
So here we can select a cellular module - in this case ah module one, and we can see immediately the last 30 minutes of cellular statistics or data right around the quality and the, and the signal strength of this link. Now that in itself can be quite useful, and we can see here that we had a small outage here WAN down, WAN up at around about (click on it, we'll see) about 12mins past five. But if we go and give it a longer time period, we can see a little bit more information, right?
Speaker 1 (09:27):
So here we have some fairly obvious changes. So between eight o'clock in the morning and around about half past one this afternoon everything was fairly stable here. So we can see which frequency it was connected to. And we can see the latency and we can see which cell tower is connected to at this stage as well. And then later we can see if the frequency has changed, which it hasn't, or indeed if the cell tower has changed, which it hasn't. So we can see that perhaps around this time, and here we are at between two and half past four, there's been considerable change to the RF environment here. Now that could be caused by a number of things I've been moving the device around as I've been filming it today. I'm I live right next to a very busy road - you can sometimes hear it in the background. So at different times of the day, when there's more traffic outside, there are more mobile phones and more cellular devices, and they definitely impact and congest the local tower. So that could be related to that as well.
New Speaker (10:35):
The key thing here though, is we can see when there's been WAN outages, and we can see when there's been a difference in cellular signal which can help explain to the customer as to what's been going on.
New Speaker (10:49):
Apart from that, I think we're, I think we've, I think that's probably it, for InControl 2 at this level. We can see that we can log into the device with Remote web admin and check real time client and and usage information. We can see historic usage information and cellular RF information, which is handy too, and at a glance, in this view, we can see whether the device is connected or not. And that as a set of capabilities is really, really helpful in providing this level of support.
New Speaker (11:27):
Thanks very much.


bright
