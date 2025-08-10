# 🔄 Network Switch Simulator

A simple, interactive tool that shows how network switches work. Learn the basics of how switches route data between devices in a network.

## 📋 Overview

### What the Simulator Does

This tool shows you how a network switch makes smart decisions about sending data. Here's what happens:

1. **Learns Device Locations**: The switch figures out where each device is connected by looking at incoming data
2. **Builds a Memory Table**: Keeps track of which devices are on which ports
3. **Routes Data Smartly**: Uses what it learned to send data directly to the right device
4. **Handles Unknown Devices**: When it doesn't know where a device is, it sends data everywhere to find it
5. **Reduces Network Traffic**: Prevents unnecessary data from going to devices that don't need it

### How Switch Functions Work

Here's the step-by-step process:

- **Starting Point**: Switch begins empty - it doesn't know where any devices are
- **First Message**: When Device A talks to Device B, the switch learns where Device A is and searches for Device B
- **Learning**: Switch remembers device locations for future use
- **Smart Routing**: Once it knows where both devices are, it creates a direct path
- **Traffic Control**: Stops sending data to devices that don't need it

## ✨ Features

### Switch Functions You'll See

#### 📚 Learning
- **When it happens**: Every time a device sends data
- **What it does**: Remembers where each device is located
- **What you'll see**: Cable lights up from the device that's sending data
- **Why it matters**: Makes future communication faster and more efficient

#### 🌊 Flooding  
- **When it happens**: When the switch doesn't know where to send data
- **What it does**: Sends data to all devices to find the right one
- **What you'll see**: Multiple cables light up at once (shown in red/orange)
- **Why it matters**: Makes sure data gets delivered even when the switch doesn't know where to send it

#### 📤 Forwarding
- **When it happens**: When the switch knows where both devices are
- **What it does**: Creates a direct path between two devices
- **What you'll see**: Only two cables light up (shown in green) - sender and receiver
- **Why it matters**: Fastest and most efficient way to send data

#### 🚫 Filtering
- **When it happens**: During normal communication between devices
- **What it does**: Blocks data from going to devices that don't need it
- **What you'll see**: Unused devices show red borders with "BLOCKED" messages
- **Why it matters**: Keeps the network clean and reduces unnecessary traffic

### MAC Address Table (Switch Memory)

The **MAC Address Table** is like the switch's address book:

- **What it stores**: Device addresses and which port they're connected to
- **How it works**: Gets filled automatically as devices talk to each other
- **How decisions are made**: Switch looks up addresses to decide where to send data
- **What happens when full**: Real switches can remember thousands of devices
- **Three types of decisions**:
  - **Known device**: Send directly to the right port
  - **Unknown device**: Send to all ports to find it
  - **Broadcast message**: Always send to everyone

## 🚀 Getting Started

### What You Need
- Any web browser (Chrome, Firefox, Safari, Edge)
- JavaScript turned on
- Works offline - no internet needed

### Setup
1. Download the `switch.html` file
2. Double-click to open it in your browser
3. Start using it right away!

## 🎮 How to Use

### Interactive Mode
• **Click on any device** (Computer, Printer, Server, or Laptop) - it turns orange when selected
• **Click on another device** to send data between them
• **Watch what happens** - see how the switch handles the communication
• **Notice the learning** - the switch remembers device locations automatically
• **Start over anytime** with the 🔄 Reset button

### Demo Mode  
• **📚 Learning Demo**: See how the switch discovers device locations
• **🌊 Flooding Demo**: Watch what happens when the switch doesn't know where to send data
• **📤 Forwarding Demo**: See direct communication between devices the switch knows
• **🚫 Filtering Demo**: Watch how unused devices get blocked from receiving data
• **📋 View MAC Table**: See what the switch has learned about device locations

### Tips for Learning
• **Start simple**: Try one communication first to see basic learning
• **Try more**: Send more messages to see how forwarding works
• **Use the demos**: The demo buttons teach specific concepts step by step
• **Check the table**: Look at what the switch remembers by viewing the MAC table
• **Experiment**: Reset and try different combinations to learn more

---

**Great for**: Anyone learning networking, students preparing for certification, or professionals wanting to understand switch basics!
