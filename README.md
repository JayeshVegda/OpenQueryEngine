# OpenQueryEngine

OpenQueryEngine is a centralized, open-source collection of curated web resources, organized by category (AI, Finance, News, Photo, Search, Shopping, Social, Video). Each category contains a JSON file and a README with a table of popular websites, their icons, codes, and URLs. The project is designed for both end-users and developers who want quick access to trusted web platforms or wish to integrate these resources into their own tools.

## Project Goals
- **Centralize**: Provide a single, well-maintained source for the most useful web platforms in each category.
- **Standardize**: Use a consistent JSON structure for easy parsing and integration.
- **Empower**: Enable developers to build launchers, dashboards, browser extensions, and more using this data.
- **Open Collaboration**: Encourage community contributions to keep the resource up-to-date and comprehensive.

## Categories

| Icon | Category | Description | Folder |
|------|----------|-------------|--------|
| ![AI](ai/icon/ai.png) | **AI** | AI chatbots and LLMs | [ai](./ai) |
| ![Finance](finance/icon/finance.png) | **Finance** | Stock & finance data | [finance](./finance) |
| ![News](news/icon/news.png) | **News & Media** | News and media sources | [news](./news) |
| ![Photo](photo/icon/photo.png) | **Photo** | Stock and creative photo sites | [photo](./photo) |
| ![Search](search/icon/search.png) | **Search** | Search engines | [search](./search) |
| ![Shopping](shopping/icon/shop.png) | **Shopping** | Online shopping platforms | [shopping](./shopping) |
| ![Social](social/icon/social.png) | **Social** | Social media platforms | [social](./social) |
| ![Video](video/icon/video.png) | **Video** | Video sharing platforms | [video](./video) |

## Example Use Cases
- **Browser Extensions**: Quickly search or open any supported platform from your browser.
- **Dashboards**: Integrate the JSON data into a productivity dashboard for one-click access.
- **Launchers**: Build a universal search/launcher tool for all your favorite web resources.
- **Educational Tools**: Use the curated lists for teaching, research, or workshops.

## Technical Details
- Each category folder contains a `category.json` file with the following structure:
  ```json
  {
    "category": {
      "name": "Category Name",
      "icon": "Images/category/icon.png",
      "websites": [
        {"name": "Website Name", "code": "shortcode", "url": "https://example.com/?q={}", "icon": "Images/category/website.png"}
      ]
    }
  }
  ```
- The `{}` in URLs is a placeholder for search queries or parameters.
- All icons are PNG, 64x64px recommended, and stored in the `icon/` subfolder of each category.

## How to Use
- Browse each category folder for a list of popular websites, their codes, and direct links.
- Use the JSON files for programmatic access or integration into your own tools.
- Each folder contains a README with a table for quick reference and more details.

## Contributing
We welcome contributions! To add or update a website:

1. Edit the relevant JSON file in the appropriate category folder.
2. Add or update the icon in the `icon/` subfolder if needed (PNG, 64x64 recommended).
3. Update the folder's README table if you add a new website.
4. Ensure all links and icons are correct and working.
5. Submit a pull request with a clear description of your changes.

### Guidelines
- Use clear, descriptive names and codes.
- Prefer official website URLs.
- Use high-quality icons (PNG, transparent background preferred).
- Keep tables and JSON files alphabetically sorted by website name if possible.

## FAQ
**Q: Can I use this data in my own project?**
A: Yes! The data is open-source and MIT licensed. Attribution is appreciated but not required.

**Q: How do I add a new website or platform?**
A: Edit the relevant JSON and README in the appropriate folder, add an icon, and submit a pull request.

**Q: What if I find an error or broken link?**
A: Please open an issue or submit a fix via pull request.

**Q: Can I suggest a new category?**
A: Yes! Open an issue to discuss new categories or major changes.

## Vision & Future Plans
- Expand to more categories (e.g., developer tools, education, health).
- Add automated tests for link and icon validation.
- Build a web UI for browsing and searching all resources.
- Support for multi-language and region-specific resources.

## License
This project is open source and available under the MIT License.

## Contact
For questions or suggestions, please open an issue or contact the maintainer.
