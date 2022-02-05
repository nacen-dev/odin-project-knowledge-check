# How does the Web work?

## Knowledge Check

- What is a Network?
  ```
  A network is a connection of computers linked together so they can communicate with each other.
  ```
- What is the Internet?
  ```
  The internet is a wire of connections of multiple networks connected with each other.
  ```
- What is an IP address?
  ```
  An IP `(Internet Protocol)` address is a unique address assigned to a computer to uniquely identify it on a network.
  ```
- What is a Router?
  ```
  A Router is a device that makes sure the data sent over the network goes to the correct recipient.
  ```
- What is an ISP?

  ```
  An ISP `(Internet Service Provider)` is a company that manages special routers that are linked with other networks.
  ```

  ```
  Connecting with your ISP you are also connecting to their network which are connected with other ISP's network in which this network is what consist the internet a connection of multiple networks.
  ```

- What are Packets and how are they used to transfer data?

  ```
  Packets are chunks of data, they are used to transfer data because a huge amount of data being transferred over a network can cause huge traffick or they could get corrupted, dropped when this happens it would be easier to replace small chunks of data.
  ```

  ```
  Packets are used so data are divided into small chunks and are sent over the network, packets will use the most optimal route over the network to travel so they can reach their destination faster.
  ```

- What is a Client?

  ```
  A client is a device that connects or access a service from a remote device(Server)
  ```

- What is a Server?

  ```
  Server is a computer that provides services, data, programs to other computers(client) over the network.
  ```

- What is a Web Page?

  ```
  A Web Page is a document that can be displayed in a Web Browser such as an HTML document, and also other documents like pdf, epub, and etc.
  ```

- What is a Web Server?

  ```
  A Web Server is a computer that host the website over the internet.
  ```

- What is a Web Browser?

  ```
  A Web Browser is a program that allows you to surf the internet and display the information you have requested to your device.


  An example is looking up a website
  ```

- What is a Search Engine?

  ```
  A Search Engine is a program that helps you to search for other web pages from other websites.
  ```

- What is a DNS Request?

  ```
  A DNS `(Domain Name System)` request also known as a DNS Query is a request for information about a domain.

  A domain is a name assigned to an IP address so we humans can easily remember how to access it instead of cryptic IP addresses.

  1. A DNS request is usually initiated when you type into your web browser a website, your computer will look first if the IP address of the domain is already stored in memory which is the `memory-cache`.

  2. If it's not stored it will ask a `Resolving Name Server` for the IP address.

  3. If the Resolving Name Server does not know what the IP address is it will instead ask the `Root Name Server`

  4. If the Root Name Server also do not know what the IP address is it will instead ask the TLD `(Top-level Domain)` Server.

  5. Finally if the TLD Server still do not know it will ask the Authoritative Name Server if it knows what is the IP then the data is sent back to your computer, but if even the Authoritative Name Server does not know the IP Address it will inform your browser that the Website you are trying to access might not exist.
  ```

- Which browser are you currently using?

  ```
  I'm using Microsoft Edge v97
  ```

- In your own words, explain what happens
  when you run a search on google.com.

  1. The web browser sends an HTTP request to the server which is google.com.

  2. Once the Server receives the request it will perform an operation based on the request to either approve or reject it then it will send the data over through the network which is through packets.

  3. Once the packets finish travelling and is successfully reassembled by the web browser then it renders the data.
