# How the web works, web protocols, and how popular services are implemented on the web

*By Nathan Kaduru*  
*Jan 18, 2025 · 6 min read*

## Table of contents
- [The Architecture of the web](#the-architecture-of-the-web)
- [Essential Web Protocols: The Language of the Web](#essential-web-protocols-the-language-of-the-web)
  - [HTTP/HTTPS](#httphttps)
  - [TCP/IP](#tcpip)
- [Popular Web Services: Real-World Examples](#popular-web-services-real-world-examples)
  - [E-commerce Platforms](#e-commerce-platforms)
  - [Social Media Platforms](#social-media-platforms)
  - [Streaming Services](#streaming-services)
- [Conclusion](#conclusion)

## Introduction

The web is something that everybody uses, different people across different locations using it for different things, but a lot of us might not understand the core of the web. The modern web might seem like a cloud where we exchange data but in reality, it's a complex ecosystem, a lot of gears are turning, protocols, services, and technologies are major parts of the web that have to work together seamlessly to deliver the experiences we take for granted. From checking social media to ordering new headphones online, understanding how the web works is crucial, and not just for people in technology. This article explores the architecture of the web, its fundamental protocols, and how popular services are implemented in today's digital world.

## The Architecture of the web

At its core, the web operates on a client to server relationship. Clients are devices like your phone or laptop that run web browsers, while servers are powerful computers that store and serve web content, basically you are the client, and you want to get something from the server. However, this simple depiction is just a way of simplifying the complex architecture that goes on behind the scenes. When a user types a website address into their browser, a couple of things happen, let's walk through them and explain the complex terms along the way.

When you search something up (e.g. howtogetagirlfriend.com), the browser first contacts DNS servers. DNS server is a fundamental component that uses the website names we input into our browsers to find the actual location of a website. A website's location is typically a string of numbers that are hard to remember, DNS makes it possible for websites to have custom names and helps clients locate these sites to find the actual location of the website.

The DNS lookup process involves multiple steps:

- Checking the browser's cache
- Querying the operating system's DNS cache
- Contacting the local DNS resolver
- Reaching out to root DNS servers
- Finally obtaining the IP address

Once the website has been located, DNS then establishes a secure connection with the web server, requests the necessary files, these files are received in tiny chunks of data until it finally assembles and displays the webpage. This process happens within milliseconds, thanks to decades of technological optimization that a lot of people appreciate enough.

### Three-Tier Architecture

Webpages typically follow something called the Three-Tier Architecture. Let's go over it and understand its principles:

1. **Presentation Layer**: This is what users interact with through their browsers, let's use the term UI, built using HTML, CSS, and JavaScript. It handles the display of information and user interface elements. Modern frameworks like React, Vue and Angular have completely transformed this layer by enabling more dynamic and responsive approach to building user interfaces.

2. **Business Layer**: Also known as the application layer, this layer contains the core logic that processes user requests, applies business rules, and coordinates data flow. It's basically responsible for what happens when you interact with a part of the UI, for example when you click the login button on an authentication page.

3. **Persistence Layer**: This layer manages data and stores information, typically a database used to maintain user information, content, and application data.

## Essential Web Protocols: The Language of the Web

### HTTP/HTTPS

HTTP/HTTPS stands for Hypertext Transfer Protocol (HTTP) is the foundation of web communication. It's something that we all see a lot, but what does it actually mean? and what role does it play in the web? When you're on a website, there are four types of requests a client can make to the server. Let's use an example of you being on a food diner website:

- **GET request**: This can be you viewing the websites menu or visiting different pages
- **POST request**: This request can be made by placing an order
- **PUT request**: This request can be made by you updating an already existing order
- **DELETE request**: This request can be made by you cancelling your order

HTTPS is a more secure version of HTTP, where the S stands for secure, it adds encryption for secure data transmission, protecting sensitive information like passwords and payment details. This security is achieved through SSL/TLS certificates that establish encrypted connections between clients and servers.

### TCP/IP

The Transmission Control Protocol/Internet Protocol (TCP/IP) is responsible for moving data from the server to the client on the internet. When a client requests for data, it breaks the data into small packets, sends them across various network paths, and reassembles them at the destination. This protocol handles everything from routing to error recovery, ensuring data integrity across the complex web of networks that make up the internet.

## Popular Web Services: Real-World Examples

### E-commerce Platforms

Modern e-commerce websites like Amazon or Shopify utilize complex architectures to handle millions of transactions:

- **Payment Processing**: They implement secure payment gateways through web services, using APIs from providers like PayPal or Stripe. These integrations must handle various payment methods, currencies, and security requirements.
- **Inventory Management**: Real-time stock updates through database synchronization, often involving multiple warehouses and suppliers
- **Personalization**: User recommendations based on browsing history and purchase patterns, powered by machine learning algorithms
- **Search Functionality**: Advanced search engines like Elasticsearch provide fast and relevant product searches
- **Cart Management**: Distributed systems maintain shopping cart states across multiple devices and sessions

### Social Media Platforms

Social platforms demonstrate sophisticated web service implementation. Using Facebook or Instagram as examples, here's how they work:

- **Authentication**: Social login services allow users to sign in using existing accounts, implementing OAuth protocols for secure authorization
- **Real-time Updates**: WebSocket protocols enable instant messaging and live feeds, maintaining persistent connections for immediate data transfer
- **Content Delivery**: Content distribution networks (CDNs) ensure fast loading of media files by storing copies closer to users
- **Data Processing**: Microservices architecture handles various functions like posts, comments, and reactions
- **Analytics**: Complex systems track user engagement and platform performance

### Streaming Services

Platforms like Netflix and Spotify showcase advanced web technologies:

- **Adaptive Streaming**: Dynamic quality adjustment based on internet speed, using protocols like HLS or DASH
- **Content Distribution**: Geographic server distribution for optimal performance
- **User Interface**: React-based front-ends for smooth user experiences
- **Recommendation Systems**: AI-powered content suggestions through specialized APIs
- **Digital Rights Management**: Systems to protect copyrighted content

## Conclusion

The web's architecture is a testament to human ingenuity, combining various protocols and technologies to create seamless digital experiences. Understanding these fundamentals is crucial for developers and technologists as we continue to build and improve on this foundation. As new technologies emerge, the web's architecture will continue to evolve, enabling even more sophisticated and powerful applications that shape our digital future.


## Link to images used in article
https://www.altexsoft.com/static/blog-post/2023/11/e1a70c23-e5c6-4322-b24b-da27f466fc60.jpg
https://media.geeksforgeeks.org/wp-content/cdn-uploads/20210204220403/Web-Application-Architecture.png