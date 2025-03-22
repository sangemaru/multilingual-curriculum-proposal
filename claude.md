# Serenichron Multilingual Curriculum Proposal Platform

## Project Overview
This project is a dynamic multilingual curriculum proposal platform designed to showcase Serenichron's advanced AI curriculum to potential educational institution partners in Romania and beyond. The platform features seamless language switching, personalized institution name insertion via URL parameters, analytics tracking, and responsive design.

## Technical Implementation

### Core Features
- **Multilingual Support**: Toggle between English and Romanian with a floating language selector
- **Institution Personalization**: Dynamic replacement of institution name throughout document via URL query parameters
- **Analytics Integration**: Google Analytics 4 and Microsoft Clarity tracking with custom event logging
- **Responsive Design**: Optimized layouts for all device sizes

### File Structure
- `index.html`: The main HTML file containing the entire application
- `assets/images/serenichron-logo.png`: Logo image for the header

### Deployment
The application is deployed at https://serenichron.com/education/ with the following RSYNC command used for deployment:

```bash
rsync -avz /path/to/local/files serenichron-portal:/srv/www/main/current/web/education/
```

## Development Guidelines

### URL Parameters
The platform supports the following URL parameters:
- `institution`: Sets the target institution name (e.g., `?institution=IT%20Step%20Academy`)

### Analytics Events
The following custom events are tracked:
- `view_proposal`: When a personalized institution proposal is viewed

### Mobile Rendering
Particular attention should be paid to mobile rendering, especially for heading elements that contain the institution name. Previous implementations had issues with unwanted line breaks between "A Proposal for" and the institution name.

## Future Enhancements
- Add additional language options (potentially Hungarian)
- Implement section-specific analytics tracking
- Develop a version suitable for email embedding

## AI-Assisted Development Process
This project was created entirely through conversational interaction with Claude AI using the Desktop Command MCP server, which provided direct filesystem and GitHub access. The development process used natural language prompting to:

1. Design the multilingual structure
2. Implement language switching functionality
3. Create dynamic institution personalization
4. Add analytics tracking
5. Fix mobile rendering issues 
6. Deploy to the production server

The entire development process from requirements gathering to deployment took less than two hours, demonstrating the efficiency of AI-assisted development with direct system access.

## Repository Management
This project is version controlled through Git, with the public repository available at: https://github.com/sangemaru/multilingual-curriculum-proposal