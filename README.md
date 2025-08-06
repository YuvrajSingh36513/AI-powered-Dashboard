# ADmyBRAND Insights Analytics Dashboard

A modern, production-ready analytics dashboard built for digital marketing agencies. Features real-time data visualization, dark/light mode, and comprehensive campaign performance tracking.

![Dashboard Preview](https://images.unsplash.com/photo-1551288049-bebda4e38f71?w=1200&h=600&fit=crop&crop=center)

## 🚀 Live Demo

**[View Live Dashboard](https://unique-madeleine-d034af.netlify.app)**

## ✨ Features

### 📊 **Core Analytics**
- **Real-time Metrics** - Revenue, Users, Conversions, Growth Rate with live updates
- **Interactive Charts** - Line charts, bar charts, and donut charts with hover effects
- **Campaign Performance Table** - Sortable, filterable data with pagination
- **Platform Distribution** - Visual breakdown of revenue by advertising platform

### 🎨 **Modern UI/UX**
- **Dark/Light Mode** - Seamless theme switching with system preference detection
- **Responsive Design** - Perfect experience on desktop, tablet, and mobile
- **Smooth Animations** - Micro-interactions, hover effects, and loading states
- **Beautiful Loading Skeletons** - Shimmer animations during data loading

### ⚡ **Advanced Features**
- **Export Functionality** - CSV export with PDF generation capability
- **Date Range Filtering** - Quick preset ranges and custom date selection
- **Real-time Updates** - Automatic data refresh every 5 seconds
- **Advanced Filtering** - Search campaigns, filter by status and platform

### 🛠 **Technical Excellence**
- **Modern Tech Stack** - React 18, TypeScript, Tailwind CSS, Recharts
- **Component Architecture** - Reusable UI components with shadcn/ui
- **Type Safety** - Full TypeScript integration with proper interfaces
- **Performance Optimized** - Lazy loading, memoization, and efficient rendering

## 🏗 **Tech Stack**

- **Frontend**: React 18 + TypeScript
- **Styling**: Tailwind CSS + CSS Custom Properties
- **UI Components**: shadcn/ui + Radix UI primitives
- **Charts**: Recharts for data visualization
- **Icons**: Lucide React
- **Build Tool**: Vite
- **Deployment**: Netlify

## 🚀 **Quick Start**

### Prerequisites
- Node.js 18+ 
- npm or yarn

### Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd admybrand-insights
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start development server**
   ```bash
   npm run dev
   ```

4. **Open your browser**
   Navigate to `http://localhost:5173`

### Build for Production

```bash
npm run build
npm run preview
```

## 📁 **Project Structure**

```
src/
├── components/          # Reusable UI components
│   ├── ui/             # shadcn/ui base components
│   ├── charts/         # Chart components
│   ├── Header.tsx      # Navigation header
│   ├── Sidebar.tsx     # Navigation sidebar
│   ├── MetricCard.tsx  # KPI metric cards
│   └── DataTable.tsx   # Advanced data table
├── data/               # Mock data and types
├── hooks/              # Custom React hooks
├── lib/                # Utility functions
├── types/              # TypeScript definitions
└── App.tsx             # Main application component
```

## 🎯 **Key Components**

### MetricCard
Displays key performance indicators with:
- Real-time value updates
- Percentage change indicators
- Color-coded status (positive/negative/neutral)
- Smooth animations and hover effects

### Interactive Charts
- **Revenue Chart**: Multi-line chart showing revenue, users, and conversions
- **Platform Chart**: Donut chart displaying revenue distribution
- **Campaign Bar Chart**: Comparative cost vs revenue analysis

### Advanced DataTable
- **Sorting**: Click column headers to sort data
- **Filtering**: Search campaigns and filter by status
- **Pagination**: Navigate through large datasets
- **Export**: Download data as CSV or PDF

## 🎨 **Design System**

### Color Palette
- **Primary**: Blue (#3B82F6) - Main brand color
- **Secondary**: Purple (#8B5CF6) - Accent elements
- **Success**: Green (#10B981) - Positive metrics
- **Warning**: Yellow (#F59E0B) - Neutral states
- **Error**: Red (#EF4444) - Negative metrics

### Typography
- **Headings**: Inter font family, multiple weights
- **Body**: Consistent line heights (150% body, 120% headings)
- **Code**: Monospace for technical elements

### Spacing System
- **Base Unit**: 8px grid system
- **Consistent Margins**: 4px, 8px, 16px, 24px, 32px, 48px
- **Component Padding**: Standardized across all cards and containers

## 📱 **Responsive Breakpoints**

- **Mobile**: < 768px - Single column layout, collapsible sidebar
- **Tablet**: 768px - 1024px - Two-column grid, condensed navigation
- **Desktop**: > 1024px - Full multi-column layout, expanded sidebar

## 🔧 **Configuration**

### Environment Variables
No environment variables required for basic setup. All data is mocked for demonstration.

### Customization
- **Colors**: Modify CSS custom properties in `src/index.css`
- **Data**: Update mock data in `src/data/mockData.ts`
- **Components**: Extend or modify components in `src/components/`

## 📊 **Data Structure**

### Metric Cards
```typescript
interface MetricCard {
  id: string;
  title: string;
  value: string;
  change: number;
  changeType: 'positive' | 'negative' | 'neutral';
  icon: string;
}
```

### Campaign Data
```typescript
interface TableRow {
  id: string;
  campaign: string;
  platform: string;
  impressions: number;
  clicks: number;
  ctr: number;
  cpc: number;
  cost: number;
  conversions: number;
  revenue: number;
  roas: number;
  status: 'active' | 'paused' | 'ended';
}
```

## 🚀 **Performance Features**

- **Code Splitting**: Automatic route-based code splitting
- **Lazy Loading**: Components loaded on demand
- **Memoization**: React.memo for expensive components
- **Optimized Rendering**: Efficient re-renders with proper dependencies

## 🔒 **Best Practices**

- **TypeScript**: Full type safety throughout the application
- **Component Composition**: Reusable, composable UI components
- **Accessibility**: ARIA labels, keyboard navigation, screen reader support
- **SEO Ready**: Proper meta tags and semantic HTML structure

## 🤝 **Contributing**

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 **License**

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 **Acknowledgments**

- **shadcn/ui** for the beautiful component library
- **Recharts** for powerful data visualization
- **Tailwind CSS** for utility-first styling
- **Lucide** for the comprehensive icon set

---

**Built with ❤️ for digital marketing agencies**
