# 📦 File Transfer Tool

A lightweight web tool for transferring files between devices using GitHub Gists. No account required, no backend needed.

## ✨ Features

- 🚀 **No Account Required** - Uses anonymous GitHub Gists
- 🔒 **No Backend** - Pure client-side JavaScript  
- 📦 **Multiple Files** - Upload several files at once
- 📋 **Easy Retrieval** - Copy or download files instantly
- ⚡ **Static Hosting** - Works on any static host (GitHub Pages, etc.)
- 🎯 **Simple** - Paste content or upload files, get a transfer ID

## 🚀 How to Use

### Sending Files:
1. Open the tool in your browser
2. Paste text content OR upload files
3. Click "Create Transfer Link"
4. **Copy the Transfer ID**

### Receiving Files:
1. Open the tool
2. Paste the Transfer ID  
3. Click "Retrieve Files"
4. Download or copy the content

## 📦 Deployment

### Local Use
Simply open `transfer.html` in any browser. No server required.

### GitHub Pages

1. Push to GitHub:
   ```bash
   git add .
   git commit -m "Deploy file transfer tool"
   git push origin main
   ```

2. Enable GitHub Pages:
   - Repository Settings → Pages
   - Source: "GitHub Actions"

3. Access at: `https://yourusername.github.io/yourrepo/`

### Other Hosts
Upload `transfer.html` to any static hosting service (Netlify, Vercel, etc.)

## 📁 Project Structure

```
├── transfer.html       # Main application (fully self-contained)
├── index.html         # Optional redirect to transfer.html
├── .github/
│   └── workflows/
│       └── deploy.yml # GitHub Actions workflow
└── README.md          # Documentation
```

## 🔒 Privacy & Security

- Files are stored as anonymous GitHub Gists
- Anyone with the transfer ID can access files
- Gists are unlisted but **not encrypted**
- **Avoid transferring sensitive information**
- Gists persist unless manually deleted

## 🛠️ Technical Details

- **API**: GitHub Gists API (`https://api.github.com/gists`)
- **Authentication**: None required (anonymous gists)
- **Framework**: Vanilla JavaScript, no dependencies
- **Storage**: GitHub's infrastructure
- **Limits**: Subject to GitHub API rate limits

## ⚠️ Limitations

- **File size**: Works best with reasonably-sized files
- **File types**: Optimized for text files (code, documents, etc.)
- **Rate limits**: GitHub API rate limits apply (sufficient for normal use)
- **Privacy**: Not suitable for confidential data

## 🆘 Troubleshooting

**"Failed to create gist"**
- Verify internet connection
- Check if GitHub API is accessible
- Wait if rate-limited (usually temporary)

**"Transfer not found"**  
- Confirm the transfer ID is correct
- Ensure the entire ID was copied
- Gist may have been deleted by owner

**Can't access tool**
- Try local version (`transfer.html` directly)
- Check if hosting service is accessible
- Use alternative browser if needed

## 📝 License

MIT License - Free to use and modify.

## 🤝 Contributing

Contributions welcome! Feel free to submit issues or pull requests.

---

Simple, secure, serverless file transfers.
