# Overview of Distributions<a name="distribution-overview"></a>

When you want to use CloudFront to distribute your content, you create a distribution and choose the configuration settings you want\. For example:
+ Your content origin—that is, the Amazon S3 bucket, AWS Elemental MediaPackage channel, or HTTP server from which CloudFront gets the files to distribute\. You can specify any combination of up to 25 Amazon S3 buckets, channels, and/or HTTP servers as your origins\. 
+ Access—whether you want the files to be available to everyone or restrict access to some users\.
+ Security—whether you want CloudFront to require users to use HTTPS to access your content\.
+ Cookie or query\-string forwarding—whether you want CloudFront to forward cookies or query strings to your origin\.
+ Geo\-restrictions—whether you want CloudFront to prevent users in selected countries from accessing your content\.
+ Access logs—whether you want CloudFront to create access logs that show viewer activity\.

For the current limit on the number of distributions that you can create for each AWS account, see [General Limits on Web Distributions](cloudfront-limits.md#limits-web-distributions) and [Limits on RTMP Distributions](cloudfront-limits.md#limits-rtmp-distributions)\. The number of files that you can serve per distribution is unlimited\.

You can use distributions to serve the following content over HTTP or HTTPS:
+ Static and dynamic download content, for example, \.html, \.css, \.js, and image files, using HTTP or HTTPS\.
+ Video on demand in different formats, such as Apple HTTP Live Streaming \(HLS\) and Microsoft Smooth Streaming\. For more information, see the [Delivering On\-Demand Video with CloudFront](on-demand-video.md)\.

  You can't serve Adobe Flash multimedia content over HTTP or HTTPS, but you can serve it using a CloudFront RTMP distribution\. See [RTMP Distributions](distribution-overview-rtmp.md)\.
+ A live event, such as a meeting, conference, or concert, in real time\. For live streaming, you create the distribution automatically by using an AWS CloudFormation stack\. For more information, see the applicable live\-streaming tutorial in [Delivering Live Streaming Video with CloudFront and AWS Media Services](live-streaming.md)\.

For information about creating a distribution, see [Steps for Creating a Distribution \(Overview\)](distribution-web-creating.md)\.