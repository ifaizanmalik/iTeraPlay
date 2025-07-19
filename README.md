# 🎬 iTeraPlay - Advanced TeraBox Video Platform

<div align="center">

<img src="https://iteraplay.com/media/logo.png" alt="iTeraPlay Logo" width="200">

**🚀 Play, Download & Stream TeraBox Videos Online**

[![Website](https://img.shields.io/badge/Website-iteraplay.com-blue?style=for-the-badge&logo=globe)](https://iteraplay.com)
[![Chrome Extension](https://img.shields.io/badge/Chrome-Extension-green?style=for-the-badge&logo=google-chrome)](https://iteraplay.com/blog/post/chrome-extension.php)
[![API Documentation](https://img.shields.io/badge/API-Documentation-orange?style=for-the-badge&logo=api)](https://iteraplay.com/blog/post/purchase-api.php)
[![Premium Plans](https://img.shields.io/badge/Premium-Plans-gold?style=for-the-badge&logo=crown)](https://iteraplay.com/pages/premium.php)

</div>

---

## 🌟 Overview

**iTeraPlay** is a comprehensive TeraBox video platform that allows users to play and download TeraBox videos directly in their browser without requiring any app installation. Built with modern PHP architecture and enhanced with advanced features for seamless video streaming.

### 🔗 Quick Links
- 🏠 **Main Website**: [iteraplay.com](https://iteraplay.com)
- 📱 **Chrome Extension**: [Download Here](https://iteraplay.com/blog/post/chrome-extension.php)
- 📖 **Download Guide**: [How to Download](https://iteraplay.com/blog/post/terabox-download-guide.php)
- 💰 **Premium Plans**: [Upgrade Now](https://iteraplay.com/pages/premium.php)
- 🔧 **API Access**: [Purchase API](https://iteraplay.com/blog/post/purchase-api.php)

---

## ✨ Key Features

### 🎥 **Video Platform**
- ▶️ **Instant Video Playback** - Play TeraBox videos directly in browser
- 📥 **Fast Downloads** - Download videos with single click
- 🖼️ **Smart Thumbnails** - Automatic thumbnail generation and caching
- 📱 **Mobile Responsive** - Optimized for all devices and screen sizes
- 🔄 **Auto-Processing** - Intelligent link processing with Cloudflare Workers

### 🚀 **Chrome Extension**
- 🔧 **One-Click Processing** - Process TeraBox links directly from browser
- 🎯 **Smart Detection** - Automatic TeraBox link recognition on any webpage
- ⚡ **Instant Access** - Skip manual copy-paste with direct processing
- 📊 **Usage Analytics** - Track your extension usage and statistics
- 🔄 **Auto-Redirect** - Seamless redirection to processed videos

### 👤 **User Management**
- 🔐 **Secure Authentication** - Ajax-powered login/signup system
- 📧 **Email Notifications** - Premium HTML welcome emails via SMTP
- 👑 **Premium Accounts** - Enhanced features and unlimited access
- 📈 **Usage Tracking** - Detailed analytics and watch history
- 🔖 **Smart Bookmarks** - Save favorite videos for later viewing

### 🛠️ **Developer Features**
- 🔌 **REST API** - Complete API for developers and businesses
- 📚 **Documentation** - Comprehensive API documentation and guides
- 🔑 **Authentication** - Secure API key management system
- 📊 **Rate Limiting** - Smart usage limits and premium tiers
- 💻 **Multiple Formats** - Support for various response formats

---

## 🎯 Core Functionality

### 📺 **Supported TeraBox Domains**
✅ terabox.com | ✅ terabox.app | ✅ terabox.fun | ✅ 1024terabox.com  
✅ 1024tera.com | ✅ 1024tera.co | ✅ 1024box.com | ✅ terafileshare.com  
✅ teraboxshare.com | ✅ teraboxapp.com | ✅ terasharelink.com | ✅ momerybox.com  
✅ 4funbox.com | ✅ 4funbox.co | ✅ mirrobox.com | ✅ nephobox.com  
✅ freeterabox.com | ✅ tibibox.com

### 🔧 **Technical Architecture**
- **Backend**: PHP 8.2+ with PDO database connections
- **Frontend**: Responsive HTML/CSS with Ajax-powered interactions  
- **Database**: MySQL with optimized queries and indexing
- **Email System**: SMTP integration with premium HTML templates
- **Cloudflare Workers**: Ultra-fast global video processing infrastructure
- **Security**: SSL encryption, CSRF protection, input validation, and rate limiting

---

## 🚀 Getting Started

### 1️⃣ **Quick Start - Website**
1. Visit [iteraplay.com](https://iteraplay.com)
2. Paste your TeraBox link in the input field
3. Click "Play Video" to start streaming instantly
4. Use "Download" button for offline viewing

### 2️⃣ **Chrome Extension Setup**
1. Visit [Chrome Extension Guide](https://iteraplay.com/blog/post/chrome-extension.php)
2. Download from Chrome Web Store
3. Install and grant necessary permissions
4. Use extension popup or auto-redirect features

### 3️⃣ **API Integration**
1. Read [API Documentation](https://iteraplay.com/blog/post/api-guide.php)
2. Purchase API access from [Premium Plans](https://iteraplay.com/pages/premium.php)
3. Get your API key and start integration
4. Follow code examples and best practices

---

## 💎 Premium Features

### 🌟 **Free vs Premium Comparison**

| Feature | Free Users | Premium Users |
|---------|------------|---------------|
| Daily Video Limit | 5 videos | ✅ Unlimited |
| Bookmark Limit | 10 bookmarks | ✅ Unlimited |
| Chrome Extension | Limited usage | ✅ Unlimited |
| API Access | ❌ Not available | ✅ Full access |
| Priority Support | ❌ Standard | ✅ Premium support |
| Ad-Free Experience | ❌ Ads shown | ✅ Completely ad-free |

### 💰 **Pricing Plans**
- **7 Days**: ₹69 - Perfect for trial and short-term use
- **30 Days**: ₹149 - Most popular for regular users
- **Lifetime**: ₹999 - Best value for power users

**[Upgrade to Premium →](https://iteraplay.com/pages/premium.php)**

---

## 🔌 Cloudflare Worker API

### 🚀 **Core Processing Engine**
Our advanced Cloudflare Worker infrastructure powers the entire platform with ultra-fast TeraBox video processing across multiple global edge locations.

### 🔑 **Example Worker Integration**
```javascript
// Example Worker API integration
const response = await fetch('https://example-worker.your-domain.workers.dev/', {
    method: 'POST',
    headers: {
        'Content-Type': 'application/json',
    },
    body: JSON.stringify({ link: teraboxUrl })
});

const data = await response.json();
// Returns: file_name, file_size, thumbnail, download_link, proxy_url
```

### 🔧 **PHP Implementation**
```php
// Server-side API call to Example Worker with cURL (recommended)
function callExampleWorker($terabox_url) {
    $workerUrl = "https://example-worker.your-domain.workers.dev/";
    
    $ch = curl_init($workerUrl);
    curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
    curl_setopt($ch, CURLOPT_POST, true);
    curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(['link' => $terabox_url]));
    curl_setopt($ch, CURLOPT_HTTPHEADER, ['Content-Type: application/json']);
    curl_setopt($ch, CURLOPT_TIMEOUT, 25);
    curl_setopt($ch, CURLOPT_CONNECTTIMEOUT, 15);
    curl_setopt($ch, CURLOPT_SSL_VERIFYPEER, false);
    curl_setopt($ch, CURLOPT_USERAGENT, 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36');

    $response = curl_exec($ch);
    $http_code = curl_getinfo($ch, CURLINFO_HTTP_CODE);
    curl_close($ch);

    if ($http_code === 200) {
        return json_decode($response, true);
    }
    return false;
}

// Alternative using file_get_contents
$postData = json_encode(['link' => $teraboxUrl]);
$context = stream_context_create([
    'http' => [
        'method' => 'POST',
        'header' => 'Content-Type: application/json',
        'content' => $postData
    ]
]);
$response = file_get_contents($workerUrl, false, $context);
```

### 📊 **Worker Response Format**
```json
{
    "file_name": "Video Title.mp4",
    "file_size": "125.4 MB", 
    "size_bytes": 131538944,
    "thumbnail": "https://thumbnail-url.jpg",
    "download_link": "https://direct-download-url",
    "proxy_url": "https://proxy-stream-url",
    "duration": "00:05:30"
}
```

### 🛠️ **Integration Examples**
```php
// Example: Process and display video
$data = callExampleWorker($teraboxUrl);
if ($data && !isset($data['error'])) {
    echo "File: " . $data['file_name'];
    echo "Size: " . $data['file_size']; 
    echo "Stream: " . $data['proxy_url'];
}
```

### ⚡ **Cloudflare Worker Features**
- **Ultra-Fast Processing**: Sub-second video link processing globally  
- **Advanced Headers**: Browser-like headers with cookie authentication
- **Size Formatting**: Automatic file size conversion (bytes to GB/MB/KB)
- **Error Handling**: Comprehensive timeout and error management
- **Multiple Domains**: Support for all TeraBox mirror domains
- **Proxy Streaming**: Direct video streaming through proxy URLs
- **Thumbnail Caching**: Automatic thumbnail generation and caching

### 🔧 **Worker Code Structure**
```javascript
// Main processing function in Cloudflare Worker
async function getFileInfo(link, request) {
  try {
    // Step 1: Fast initial fetch with 5 second timeout
    const response = await fetch(link, { 
      headers: HEADERS,
      signal: AbortSignal.timeout(5000)
    });
    
    // Step 2: Extract surl parameter
    const finalUrl = response.url;
    const url = new URL(finalUrl);
    const surl = url.searchParams.get("surl");
    
    // Step 3: Make API call to get file data
    const apiResponse = await fetch(`https://dm.1024tera.com/share/list?...`);
    const data = await apiResponse.json();
    
    return {
      file_name: data.server_filename,
      file_size: getSize(data.size),
      thumbnail: data.thumbs?.url4 || data.thumbs?.url3,
      download_link: data.dlink,
      proxy_url: `${PROXY_BASE_URL}/${data.fs_id}`
    };
  } catch (error) {
    return { error: error.message };
  }
}
```

### 📚 **Complete API Documentation**
For detailed API documentation, pricing, and purchase:
**[Purchase API Access →](https://iteraplay.com/blog/post/purchase-api.php)**

---

## 📱 Mobile Apps & Extensions

### 🌐 **Chrome Extension**
- **Download**: [Chrome Web Store Extension](https://iteraplay.com/blog/post/chrome-extension.php)
- **Features**: Auto-detection, one-click processing, unlimited access for premium users
- **Supported**: All major TeraBox domains and mirror sites
- **Guide**: [Extension Setup Guide](https://iteraplay.com/blog/post/chrome-extension-guide.php)

### 📱 **iOS Shortcut** 
- **Download**: [iOS Shortcut Guide](https://iteraplay.com/blog/post/ios-shortcut.php)
- **Features**: Share sheet integration, automatic processing, native iOS experience
- **Compatibility**: iPhone, iPad, Mac with iOS 13+

### 🤖 **Telegram Bot**
- **Access**: [@iteraplay_bot](https://t.me/iteraplay_bot)
- **Features**: Direct video processing via Telegram messages
- **Usage**: Send TeraBox links directly to bot for instant processing
- **Tutorial**: [Create Your Own Bot](https://iteraplay.com/blog/post/make-your-own-telegram-bot.php)

---

## 📖 Comprehensive Guides

### 📝 **Step-by-Step Tutorials**
1. **[Chrome Extension Guide](https://iteraplay.com/blog/post/chrome-extension-guide.php)** - Detailed extension setup and usage
2. **[TeraBox Download Guide](https://iteraplay.com/blog/post/terabox-download-guide.php)** - Best practices for downloading videos
3. **[Create Your Own TeraBox Website](https://iteraplay.com/blog/post/make-your-own-terabox-website.php)** - Developer tutorial
4. **[Make Your Own Telegram Bot](https://iteraplay.com/blog/post/make-your-own-telegram-bot.php)** - Bot development guide

### 🔧 **Technical Resources**
- **[Developer Blog](https://iteraplay.com/blog/)** - Latest updates and technical insights
- **[API Purchase](https://iteraplay.com/blog/post/purchase-api.php)** - Get API access for developers
- **[Support Center](https://iteraplay.com/pages/contact.php)** - Get help and report issues
- **[Premium Support](https://iteraplay.com/pages/premium.php)** - Priority support for premium users

---

## 🌟 Community & Support

### 💬 **Get Connected**
- 🤖 **Telegram Bot**: [@iteraplay_bot](https://t.me/iteraplay_bot)
- 📧 **Email Support**: [Contact Us](https://iteraplay.com/pages/contact.php)
- 💰 **Support**: [Contact Us](https://iteraplay.com/pages/contact.php)

### 🆘 **Need Help?**
1. Check our [comprehensive guides](https://iteraplay.com/blog/)
2. Contact support via [contact page](https://iteraplay.com/pages/contact.php)
3. Join our Telegram bot for quick assistance
4. Premium users get priority support

---

## 📊 Platform Statistics

<div align="center">

[![Platform Stats](https://img.shields.io/badge/Users-1000%2B-brightgreen?style=for-the-badge)](https://iteraplay.com)
[![Videos Processed](https://img.shields.io/badge/Videos_Processed-10000%2B-blue?style=for-the-badge)](https://iteraplay.com)
[![Uptime](https://img.shields.io/badge/Uptime-99.9%25-success?style=for-the-badge)](https://iteraplay.com)
[![Response Time](https://img.shields.io/badge/Response_Time-%3C2s-orange?style=for-the-badge)](https://iteraplay.com)

</div>

---

## 🔐 Privacy & Security

### 🛡️ **Security Features**
- ✅ **SSL Encryption** - All data transmitted securely
- ✅ **No Data Storage** - Videos processed in real-time, not stored
- ✅ **Privacy First** - Minimal data collection, GDPR compliant
- ✅ **Secure Authentication** - Industry-standard security practices

### 📋 **Privacy Policy**
We respect your privacy and handle data responsibly. Read our complete privacy policy on the website.

---

## 🚀 Latest Updates

### 🎉 **Recent Improvements** (July 2025)
- ⚡ **Performance Boost** - 50% faster video processing with Cloudflare optimization
- 🎨 **UI Enhancement** - Modern dark theme with improved user experience
- 🔧 **Chrome Extension v5.11** - Enhanced with smart rating system and unlimited access
- 📱 **Mobile Optimization** - Better responsive design for mobile devices
- 🔗 **SEO Improvements** - Enhanced search engine visibility and structured data

---

## 🌍 Global Reach

**iTeraPlay** serves users worldwide with:
- 🌐 **Multi-language Support** - Interface available in multiple languages
- ⚡ **Global CDN** - Fast loading times worldwide via Cloudflare
- 📱 **Cross-Platform** - Works on all devices and operating systems
- 🔄 **24/7 Availability** - Round-the-clock service with 99.9% uptime

---

<div align="center">

## 🎯 Start Using iTeraPlay Today!

**[🚀 Visit Website](https://iteraplay.com) | [📱 Get Extension](https://iteraplay.com/blog/post/chrome-extension.php) | [💎 Go Premium](https://iteraplay.com/pages/premium.php) | [🔧 API Access](https://iteraplay.com/blog/post/purchase-api.php)**

---

### Built with ❤️ for the TeraBox community

**© 2025 iTeraPlay. All rights reserved.**

[Website](https://iteraplay.com) • [Premium](https://iteraplay.com/pages/premium.php) • [API](https://iteraplay.com/blog/post/purchase-api.php) • [Support](https://iteraplay.com/pages/contact.php)

</div>