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

### Icons

[icon-collection](https://github.com/metaory/icon-collection/tree/master/logo) - curated logos for Slack emojis.

## Usage

```bash
emoji-util list                           # List all emojis
emoji-util del NAME                       # Delete specific emoji
emoji-util del-all [SLEEP]                # Delete all emojis
emoji-util create NAME PATH               # Create single emoji from file
emoji-util create-all PATH [SLEEP] [LOG]  # Create emojis from directory
```

### Examples

```bash
# Create single emoji
emoji-util create tmux ~/dev/icon-collection/logo/tmux.png
emoji-util create lambda-1 ~/dev/icon-collection/logo/lambda-1.png

# Create all emojis from directory
emoji-util create-all ~/dev/icon-collection/logo

# List all emojis
emoji-util list
```

---

## License

[MIT](LICENSE)
