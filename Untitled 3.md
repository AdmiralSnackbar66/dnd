---
type: 'training provider'  
tags: ['training', 'provider']  
website: 'https://www.pluralsight.com'  
title: 'Pluralsight'  
---

```dataviewjs  
   let pg = dv.current(); // set pg to be the current page, for brevity  
    
   dv.header(1, pg.title); // print the page title from YAML as H1  
   dv.header(2, 'Website'); // print 'Website' as an H2  
   dv.paragraph(pg.website) // print website url from YAML in a paragraph  
      
   dv.header(2, 'Courses Taken:'); // print 'Courses Taken' as an H2  
   dv.list(dv.pages('#training').where(p => p.provider && p.provider.contains(pg.title)).file.link);  
```