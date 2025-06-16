# ClusterScope - Interactive Cluster Visualization Tool

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![D3.js](https://img.shields.io/badge/D3.js-F9A03C?logo=d3.js&logoColor=white)](https://d3js.org/)

> A powerful, interactive web-based tool for visualizing and exploring dimensional reduction results from any machine learning algorithm.

## 🌐 **[Try ClusterScope Live!](https://yourusername.github.io/clusterscope/)**

## 📝 Citation

If you use **ClusterScope** in your research or teaching, please cite it as:

Terenzi, M. (2025). *ClusterScope: Interactive Cluster Visualization Tool* (Version 1.0) [Computer software]. GitHub. https://github.com/yourusername/clusterscope

```bibtex
@software{terenzi2025clusterscope,
  author = {Terenzi, M.},
  title = {ClusterScope: Interactive Cluster Visualization Tool},
  year = {2025},
  version = {1.0},
  url = {https://github.com/yourusername/clusterscope},
  note = {Computer software}
}
```

[![DOI](https://zenodo.org/badge/1003260131.svg)](https://doi.org/10.5281/zenodo.15678529)

## 🚀 Features

### Universal Algorithm Support
- **UMAP** - Uniform Manifold Approximation and Projection
- **t-SNE** - t-Distributed Stochastic Neighbor Embedding  
- **PCA** - Principal Component Analysis
- **ICA** - Independent Component Analysis
- **MDS** - Multidimensional Scaling
- **Custom algorithms** - Any 2D coordinate system

### Interactive Visualization
- 🔍 **Smart zoom controls** with pan and selection modes
- 🎨 **Dynamic point sizing** based on zoom level
- 📊 **Cluster filtering** - click to isolate specific clusters
- 🖱️ **Point selection** - click any data point for detailed analysis
- 📱 **Responsive design** - works on desktop and mobile

### Intelligent Data Processing
- 🧠 **Automatic column detection** - recognizes coordinate formats
- 📁 **Drag & drop CSV loading** with robust parsing
- 🏷️ **Flexible labeling** - supports various naming conventions
- 🖼️ **Image integration** - display images linked to data points
- 📈 **Real-time statistics** - dataset overview and filtered views

## 📊 Quick Start

### Option 1: Use Online (Recommended)
**[🌐 Open ClusterScope in your browser](https://yourusername.github.io/clusterscope/)**

No download required! Just prepare your CSV and start exploring.

### Option 2: Download Locally
```bash
git clone https://github.com/yourusername/clusterscope.git
cd clusterscope
# Open index.html in your browser
```

### 3. Prepare Your Data
Create a CSV file with the following structure:

#### Required Columns:
- **Coordinates**: `UMAP1/UMAP2`, `tsne1/tsne2`, `PC1/PC2`, `x/y`, etc.
- **Cluster**: `cluster`, `label`, `group`, `category`
- **File URL**: `file_url`, `image_url`, `url`, `path`

#### Optional Columns:
- **Text**: `text`, `content`, `description`, `caption`
- **Description**: `description`, `summary`, `details`

### 4. Load and Explore
1. Click "📁 Load CSV File"
2. Select your data file
3. Interact with the visualization!

## 📋 Data Format Examples

### UMAP Results
```csv
cluster,UMAP1,UMAP2,file_url,text,description
1,-2.45,1.23,https://example.com/img1.jpg,Sample text,Detailed description
2,0.87,-1.56,https://example.com/img2.jpg,Another sample,More details
3,1.34,2.78,https://example.com/img3.jpg,Third example,Additional info
```

### t-SNE Results
```csv
cluster,tsne1,tsne2,file_url,description
1,15.2,-8.7,https://drive.google.com/file/d/123abc,First cluster description
2,-12.4,5.9,https://drive.google.com/file/d/456def,Second cluster description
3,3.1,14.8,https://drive.google.com/file/d/789ghi,Third cluster description
```

### PCA Results
```csv
cluster,PC1,PC2,file_url,text
1,0.45,-0.23,path/to/image1.png,Principal component analysis result
2,-0.12,0.67,path/to/image2.png,Another PCA data point
3,0.78,0.34,path/to/image3.png,Third PCA result
```

## 🛠️ Technical Details

### Built With
- **Frontend**: HTML5, CSS3, JavaScript (ES6+)
- **Visualization**: D3.js v7
- **Data Processing**: Papa Parse
- **Design**: Custom CSS with modern UI principles

### Browser Support
- ✅ Chrome 80+
- ✅ Firefox 75+
- ✅ Safari 13+
- ✅ Edge 80+

### Performance
- Handles datasets up to **100k+ data points**
- Smooth interactions with **dynamic rendering**
- Memory-efficient **zoom and pan operations**

## 🎯 Use Cases

### Machine Learning Research
- Visualize embedding spaces from neural networks
- Compare different dimensional reduction techniques
- Analyze clustering results interactively

### Data Science Projects
- Explore high-dimensional dataset structures
- Present findings with interactive visualizations
- Quality control for ML pipeline outputs

### Academic Research
- Publication-ready visualizations
- Interactive data exploration for papers
- Educational demonstrations of ML concepts

### Business Analytics
- Customer segmentation analysis
- Product recommendation insights
- Market research visualization

## 🚀 Advanced Features

### Zoom Controls
- **Pan Mode** (`↔`): Navigate around the visualization
- **Selection Mode** (`⬚`): Draw rectangles to zoom into specific areas
- **Zoom In/Out** (`+/-`): Precise zoom control
- **Reset View** (`⌂`): Return to full dataset view

### Cluster Management
- Click any cluster in the legend to **isolate** it
- Click again to **show all clusters**
- Real-time statistics update for filtered views

### Image Integration
- Supports **Google Drive** links (automatic ID extraction)
- Direct image URLs
- Fallback loading for robust image display
- Loading states and error handling

## 🤝 Contributing

We welcome contributions! Here's how you can help:

1. **Fork** the repository
2. **Create** a feature branch (`git checkout -b feature/AmazingFeature`)
3. **Commit** your changes (`git commit -m 'Add some AmazingFeature'`)
4. **Push** to the branch (`git push origin feature/AmazingFeature`)
5. **Open** a Pull Request

### Development Guidelines
- Follow existing code style
- Add comments for complex logic
- Test with various data formats
- Ensure mobile responsiveness

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **D3.js** - For powerful visualization capabilities
- **Papa Parse** - For robust CSV parsing
- **Modern CSS** - For responsive design principles
- **Open Source Community** - For inspiration and best practices

## 📞 Support

- 🐛 **Bug Reports**: [Open an issue](https://github.com/yourusername/clusterscope/issues)
- 💬 **Questions**: [Ask in Discussions](https://github.com/yourusername/clusterscope/discussions)

---

<div align="center">

**[🌐 Try ClusterScope Live](https://yourusername.github.io/clusterscope/) | Made with ❤️ for the data science community**

[⭐ Star this repo](https://github.com/yourusername/clusterscope) | [🍴 Fork it](https://github.com/yourusername/clusterscope/fork) | [📖 Read the docs](https://github.com/yourusername/clusterscope/wiki)

</div>
