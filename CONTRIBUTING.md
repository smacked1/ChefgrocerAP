# Contributing to ChefGrocer

Thank you for your interest in contributing to ChefGrocer! This document provides guidelines and information for contributors.

## 🌟 Ways to Contribute

### 1. Code Contributions
- Bug fixes and improvements
- New features and enhancements
- Performance optimizations
- Documentation updates

### 2. Non-Code Contributions
- Recipe content and suggestions
- UI/UX design improvements
- Marketing and social media
- Testing and quality assurance
- Translation and localization

### 3. Community Support
- Help other users in discussions
- Report and verify bugs
- Suggest new features
- Share feedback and ideas

## 🛠️ Development Setup

### Prerequisites
- Node.js 18+
- Git
- PostgreSQL database
- Code editor (VS Code recommended)

### Getting Started
1. Fork the repository
2. Clone your fork: `git clone https://github.com/yourusername/chefgrocer.git`
3. Install dependencies: `npm install`
4. Set up environment variables (see README.md)
5. Start development server: `npm run dev`

### Environment Setup
Create a `.env` file with required API keys:
```env
DATABASE_URL=your_postgresql_url
GEMINI_API_KEY=your_google_gemini_key
SPOONACULAR_API_KEY=your_spoonacular_key
STRIPE_SECRET_KEY=your_stripe_secret_key
VITE_STRIPE_PUBLIC_KEY=your_stripe_public_key
```

## 📝 Code Guidelines

### TypeScript Standards
- Use TypeScript for all new code
- Define proper interfaces and types
- Avoid `any` type unless absolutely necessary
- Use proper null checking and optional chaining

### React Best Practices
- Use functional components with hooks
- Implement proper error boundaries
- Follow React performance best practices
- Use proper component composition

### Styling Guidelines
- Use Tailwind CSS for styling
- Follow existing design system
- Ensure responsive design
- Maintain accessibility standards

### API Development
- Use proper HTTP status codes
- Implement input validation
- Add rate limiting where appropriate
- Document API endpoints

## 🔧 Project Structure

```
ChefGrocer/
├── client/
│   ├── src/
│   │   ├── components/     # Reusable UI components
│   │   ├── pages/         # Application pages
│   │   ├── hooks/         # Custom React hooks
│   │   ├── lib/           # Utilities and configurations
│   │   └── types/         # TypeScript type definitions
├── server/
│   ├── services/          # External API integrations
│   ├── middleware/        # Express middleware
│   ├── routes.ts          # API route definitions
│   └── storage.ts         # Database operations
├── shared/
│   └── schema.ts          # Shared TypeScript schemas
└── docs/                  # Documentation files
```

## 🐛 Bug Reports

### Before Reporting
1. Check existing issues to avoid duplicates
2. Test with the latest version
3. Reproduce the bug consistently
4. Gather relevant information

### Bug Report Template
```markdown
**Bug Description**
A clear description of the bug

**Steps to Reproduce**
1. Go to '...'
2. Click on '...'
3. Scroll down to '...'
4. See error

**Expected Behavior**
What you expected to happen

**Actual Behavior**
What actually happened

**Environment**
- Device: [e.g., iPhone 14, MacBook Pro]
- OS: [e.g., iOS 16, macOS 13]
- Browser: [e.g., Safari, Chrome]
- Version: [e.g., 1.0.0]

**Screenshots**
Add screenshots if applicable

**Additional Context**
Any other relevant information
```

## 💡 Feature Requests

### Before Requesting
1. Check if the feature already exists
2. Search existing feature requests
3. Consider if it fits the project scope
4. Think about implementation complexity

### Feature Request Template
```markdown
**Feature Description**
A clear description of the requested feature

**Problem Statement**
What problem does this feature solve?

**Proposed Solution**
How should this feature work?

**Alternatives Considered**
Other solutions you've considered

**Additional Context**
Screenshots, mockups, or examples
```

## 🔄 Pull Request Process

### Before Submitting
1. Create a feature branch from `main`
2. Make your changes with clear commits
3. Test your changes thoroughly
4. Update documentation if needed
5. Ensure code follows style guidelines

### Pull Request Template
```markdown
**Description**
Brief description of changes

**Type of Change**
- [ ] Bug fix
- [ ] New feature
- [ ] Breaking change
- [ ] Documentation update

**Testing**
- [ ] Unit tests pass
- [ ] Integration tests pass
- [ ] Manual testing completed

**Checklist**
- [ ] Code follows style guidelines
- [ ] Self-review completed
- [ ] Documentation updated
- [ ] No new warnings introduced
```

### Review Process
1. Maintainers will review your PR
2. Address any feedback or requests
3. Once approved, your PR will be merged
4. Your contribution will be credited

## 🧪 Testing

### Running Tests
```bash
# Run all tests
npm test

# Run tests in watch mode
npm run test:watch

# Run tests with coverage
npm run test:coverage
```

### Writing Tests
- Write unit tests for new functions
- Add integration tests for API endpoints
- Test React components with React Testing Library
- Mock external dependencies appropriately

### Test Guidelines
- Test files should end with `.test.ts` or `.test.tsx`
- Use descriptive test names
- Follow AAA pattern (Arrange, Act, Assert)
- Test both success and error cases

## 📚 Documentation

### Documentation Standards
- Use clear, concise language
- Include code examples where helpful
- Keep documentation up to date
- Use proper markdown formatting

### Types of Documentation
- Code comments for complex logic
- README files for setup and usage
- API documentation for endpoints
- User guides for features

## 🎨 Design Guidelines

### UI/UX Principles
- Maintain consistency across the app
- Prioritize accessibility and usability
- Follow mobile-first design approach
- Use the established color scheme and typography

### Design Resources
- Use Unsplash for food photography
- Follow Material Design principles
- Maintain brand colors: Green (#10b981), Orange (#f97316)
- Ensure 4.5:1 color contrast ratio minimum

## 🔐 Security Guidelines

### Security Best Practices
- Never commit API keys or secrets
- Validate all user inputs
- Use parameterized queries for database
- Implement proper authentication checks
- Follow OWASP security guidelines

### Reporting Security Issues
For security vulnerabilities, please email dxmylesx22@gmail.com directly instead of creating a public issue.

## 📄 License

By contributing to ChefGrocer, you agree that your contributions will be licensed under the MIT License.

## 🤝 Code of Conduct

### Our Standards
- Be respectful and inclusive
- Welcome diverse perspectives
- Focus on constructive feedback
- Help others learn and grow
- Maintain professional communication

### Unacceptable Behavior
- Harassment or discrimination
- Offensive or inappropriate language
- Personal attacks or trolling
- Spam or self-promotion
- Violation of privacy

### Enforcement
Community guidelines violations should be reported to dxmylesx22@gmail.com. All reports will be reviewed and appropriate action will be taken.

## 📞 Getting Help

### Resources
- **Documentation**: Check the README and docs folder
- **Issues**: Search existing issues for solutions
- **Discussions**: Join community discussions
- **Email**: Contact dxmylesx22@gmail.com for direct support

### Community Channels
- GitHub Discussions for general questions
- GitHub Issues for bugs and feature requests
- Email for security issues and private matters

## 🙏 Recognition

Contributors will be recognized in:
- README.md contributors section
- Release notes for significant contributions
- Annual contributor highlights
- Special mentions in app credits

Thank you for helping make ChefGrocer better for everyone! 🍳