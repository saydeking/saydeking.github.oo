---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: Biography
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  - block: accomplishments
    content:
      # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
      title: 'News'
      subtitle:
      # Date format: https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Accomplishments.
      #   Add/remove as many `item` blocks below as you like.
      #   `title`, `organization`, and `date_start` are the required parameters.
      #   Leave other parameters empty if not required.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - certificate_url: 
          date_end: ''
          date_start: '2022-10-25'
          description: ''
          organization: PhD Progress
          organization_url: 
          title: Became a Ph.D. Candidate!
          url: 'https://www.linkedin.com/posts/saydeking_phdjourney-activity-6991044883654303744-8LQ1?utm_source=share&utm_medium=member_desktop'
        - certificate_url: 
          date_end: ''
          date_start: '2022-05-01'
          description: Awarded a Ph.D. Employer Fellowship from the National GEM Consortium sponsored by the MIT Lincoln Laboratory.
          organization: National GEM Consortium | MITLL
          organization_url: https://www.gemfellowship.org/
          title: Named a National GEM Consortium Fellow
          url: https://www.ll.mit.edu/news/sayde-king-selected-gem-phd-fellowship-lincoln-laboratory
        - certificate_url: 
          date_end: ''
          date_start: '2022-04-01'
          description: 'I was a guest on the Modern Figures podcast! In my episode, Big Brain Energy, I discuss my PhD journey and how the Modern Figures Podcast played a critical role. Have a listen!'
          organization: 
          organization_url: https://www.datacamp.com
          title: 'Featured on the Modern Figures Podcast!'
          url: 'https://modernfigurespodcast.com/big-brain-energy-episode-038/'
    design:
      columns: '2'
      
  - block: portfolio
    id: projects
    content:
      title: Selected Projects
      filters:
        folders:
          - project
      # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below)
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
  - block: collection
    id: featured
    content:
      title: Featured Publications
      filters:
        folders:
          - publication
        featured_only: true
    design:
      columns: '2'
      view: card
  - block: collection
    content:
      title: Recent Publications
      text: |-
        {{% callout note %}}
        Quickly discover relevant content by [filtering publications](./publication/).
        {{% /callout %}}
      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '2'
      view: citation

---
