# GetLatestTikTokVideoData

*Auto‑syncs your TikTok & Instagram videos: fetches latest video info and pushes new clips from your server.*

---

## Features

* **Latest Video Info**: Automatically retrieve metadata (views, likes, captions, timestamps) for your TikTok and Instagram accounts each day.
* **Remote Video Upload**: Push videos hosted on your own server to your TikTok/Instagram profile via the official Content Posting API.
* **Sandbox Mode Support**: Build and test in TikTok’s sandbox environment before going live.
* **Battle Visuals Integration**: (Optional) Generate daily “battle” videos comparing follower counts, engagements, or any custom metrics.

---

## Getting Started

1. **Clone the repository**

   ```bash
   git clone https://github.com/yourusername/YourAppName.git
   cd YourAppName
   ```

2. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

3. **Configure Environment**

   * Copy `.env.example` to `.env` and fill in your credentials:

     ```ini
     TIKTOK_CLIENT_KEY=your_tiktok_client_key
     TIKTOK_CLIENT_SECRET=your_tiktok_client_secret
     INSTAGRAM_APP_ID=your_instagram_app_id
     INSTAGRAM_APP_SECRET=your_instagram_app_secret
     SERVER_VIDEO_BASE_URL=https://yourserver.com/videos/
     ```

4. **Run in Sandbox Mode**

   * Ensure your app is toggled to **Sandbox** in the TikTok Developer Console.
   * Add your test account to the sandbox settings.

5. **Fetch Latest Video Info**

   ```bash
   python scripts/fetch_latest_videos.py
   ```

6. **Upload Video from Server**

   ```bash
   python scripts/upload_video.py --filename example.mp4
   ```

---

## Useful Links

* [Terms of Service](https://yourusername.github.io/terms.md)
* [Privacy Policy](https://yourusername.github.io/privacy.md)
* [TikTok Developer Documentation](https://developers.tiktok.com/)
* [Instagram Graph API Documentation](https://developers.facebook.com/docs/instagram)

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Contact

For support or questions, email [support@yourdomain.com](mailto:support@yourdomain.com).
