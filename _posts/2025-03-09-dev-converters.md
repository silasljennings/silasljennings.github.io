---
layout: post
title: Dev Converters
subtitle: 
thumbnail-img: /assets/img/devconverters/devconverters-logo.png
share-img: /assets/img/devconverters/devconverters-logo.png
tags: [devconverters, React, NextJS, Tailwind, Conversion Tools, Cashboard App ]
comments: true
mathjax: true
author: Luke Jennings
---

# Dev Converters: Simplifying Development Workflows with a Multi-Utility Web Conversion Tool

![Dev Converters Image](/assets/img/devconverters/devconverters-page.png)

## Overview

[Dev Converters](https://www.devconverters.com/) is an all-purpose web utility designed to simplify common tasks that developers and tech enthusiasts face on a daily basis. Whether you're working on converting timestamps into human-readable formats, translating JWT token properties, identifying geolocation metadata, or converting between file types, Dev Converters is a one-stop solution. This versatile tool brings a wide variety of conversions and integrations into a single, easy-to-use platform with one input field.

## Why I Built Dev Converters

I created Dev Converters as a direct response to the challenges I encountered while developing for my startup, [Cashboard App Inc](https://www.cashboardapp.co/) In short, the Cashboard app allows companies to schedule offer lotteries for their products at any selected location. During the development process, I frequently needed to validate various aspects of the technology, such as timestamp formatted data and geo coordinates used for the locations of the lotteries. I also had to generate fake data that utilized these same types to simulate the delivery of the products in the lotteries.

The tools I was using for this validation were spread across multiple websites. Here are just a few that I used regularly:
- [Epoch Converter](https://www.epochconverter.com/)
- [Movable Type Geohash Script](https://www.movable-type.co.uk/scripts/geohash.html)
- [Google Maps](https://www.google.com/maps)
- [JWT.io](https://jwt.io/)
- [Timestamp Converter](https://www.timestamp-converter.com/)

However, the constant switching between these sites was time-consuming and counterintuitive. As every developer knows, browser tab real estate is precious, and toggling between multiple tools can disrupt the workflow. To solve this, I combined the functionality of these pages into a single, integrated platform, which drastically streamlined my development process.

What I found particularly helpful was the intuitive layer I built into the tool. Rather than requiring users to fill out multiple fields for different conversion tasks, I implemented a smart input field that dynamically detects the type of conversion based on the input. This means that the tool can automatically recognize whether the user is entering a timestamp, geolocation, JWT token, or file, and adjust accordingly. This design not only simplifies the user experience but also makes the tool highly flexible and extensible. As a result, I can easily add new conversion types without complicating the interface, keeping it clean and easy to use for everyone.

This capability was proven when file conversions were seamlessly integrated into the tool—something I hadn’t originally planned. The flexibility of the platform allowed me to quickly incorporate a wide range of file conversions, such as:
- **Document Conversions**: Docx to PDF, Docx to TXT, DOC to PDF, and more.
- **Spreadsheet Conversions**: XLS to CSV, XLS to PDF, CSV to XLSX, and more.
- **Presentation Conversions**: PPTX to PDF, PPT to PPTX, and more.
- **Other Formats**: ODG to SVG, ODG to SWF, and more.

And this is just the beginning. I’m planning to expand Dev Converters with support for other multimedia file types, along with commonly used conversions for web assets like YouTube videos or Instagram content. By streamlining my development with this tool, I’ve not only saved valuable time but also built a platform that’s designed to evolve to meet a plethora of user needs.

## How I Built Dev Converters

Building Dev Converters involved leveraging a modern tech stack that simplified the process from start to finish. The backend of the application was built using **Next.js**, a framework I had never used before. I was pleasantly surprised at how simple it was to deploy the application using **Vercel**. I was able to purchase the domain name **devconverters.com** and easily map it to the deployed application through Vercel's interface.

For the frontend, I turned to **React**—a framework that was new to me but proved to be easy to learn and integrate. React's component-based architecture made it straightforward to manage different conversion types and their respective interfaces, and its integration with **Tailwind CSS** was especially useful; allowing me to quickly style the components and ensure responsiveness across devices without the usual complexity. This ultimately saved me a significant amount of time compared to other frameworks I've used in the past. It is definitely a framework I will be using again.

For the file conversion aspect, I used the **Jod Converter** repository, which provides a Docker service for converting office files. By deploying this via **Google Cloud Run**, I was able to offload the file conversion process to a scalable containerized service, allowing Dev Converters to handle complex file conversions seamlessly. This was my first real experience with deploying a service-based containerized application, and I plan to write another blog post discussing how this deployment expanded my understanding of the power of containers in modern app development.

## Future Improvements and Features

While Dev Converters is already a robust tool, there's still much room for growth. Here are some of the exciting features I plan to add in the future:

1. **Support for Multimedia File Conversions**  
   I’m working on adding support for converting multimedia file types like audio and video formats (MP3, MP4, WAV, etc.) into different formats.

2. **YouTube Link Conversions**  
   Converting YouTube links to useful resources, such as thumbnails or extracting the audio from videos, is another feature I’d like to implement.

3. **Additional Conversion Types**  
   I also plan to expand the tool with more conversions related to file size, speed, distance, and other commonly used conversions.

4. **Command-Line Utility**  
   As Dev Converters continues to grow in popularity, a command-line utility version of the tool could be a game-changer for developers looking to automate their workflow and speed up processes.

5. **AI Generated Conversions**  
   Integrating AI technologies with natural language processing to make the interface even more intuitive for the conversion processing.

## Conclusion

Dev Converters is a tool born out of necessity, designed to simplify tasks that developers encounter regularly. By combining multiple utilities into one platform, it helps save time and increase productivity. With the power of Next.js, React, Tailwind CSS, and Google Cloud Run, Dev Converters is both easy to use and scalable for future enhancements. As I continue to improve and add more conversion types, hopefully this tool will become an invaluable resource for developers everywhere.
