EMOJI-UTIL
==========

Slack emoji management utility - simple CRUD operations on Slack admin API.

**No Slack Enterprise or Slack App required** - works with any regular Slack workspace.

## Setup

1. Go to your Slack workspace emoji admin page
2. Open browser dev tools (F12) → Network tab
3. Click on emoji list or any emoji action
4. Right-click on the request → Copy → Copy as cURL
5. Save it to `curl-request` file:
   ```bash
   cp curl-request.sample curl-request
   # Edit curl-request with your copied curl command
   ```

## Usage

```bash
emoji-util list                    # List all emojis
emoji-util del NAME               # Delete specific emoji
emoji-util del-all [SLEEP]        # Delete all emojis
emoji-util create NAME [PATH]     # Create single emoji
emoji-util create-all PATH [SLEEP] # Create emojis from directory
```

---

## License

[MIT](LICENSE)
