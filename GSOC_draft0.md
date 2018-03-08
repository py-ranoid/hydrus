# About me

Hello world.
I'm Vishal, a 3rd yr CSE undergrad from Chennai, India. While most people generally pick up a topic, or a concept (like say Computer Vision, Big Data, or just Algorithms), understand it and aspire to excel at it... I fell in love with a language, _Python_. As someone who has started out by learning C++ in school, learning Python was as easy as surprising. The speed at which I could translate ideas to code was amazing, and oh boy, all I wanted to do was make things, write simple scripts to automate everyday tasks. And hence I continued to explore Python, the countless modules and possibilities with Python. I went to Hackathons, won some but more importantly made something that others could use. And I guess that's always been my mantra for programming and my way to "help the world" : Make cool stuff. <br> And since awesomeness is universal and often found in Github repos, I dived into open-source, an ocean of cool stuff that could potentially be made _cooler_.

### Projects I've done relevant to this proposal
- Used Django, Celery and other Python modules to develop this : www.pygeon.tech
    - Hackathons and Developer events are hard to keep track of
    - Used celery to scrape events from some sites every day
    - Used Messenger as a medium to keep subscribers updated with new events as and when they're found
    - Used Docker to deploy
- Developed a chatbot for a Startup, which was deployed with Django on an EC2 instance
- Taught 45 freshers in my college, the basics of Flask, application, context and REST API
### Contributions to Hydrus
- Code cleansing and debugging.
    - Removed unused pdb imports
        - Raised 3 PRs #107, #108 and #109 (Merged)
    - Corrected Item insertion message in app.py
        - Raised PR #146 (Merged)
    - Raised issue to distinguish between incorrect and missing credentials (Issue #152)
        - Being resolved in PR #144
- Added documentation. (Issue #98)
    - Documented hydrus/utils.py (PR #138 and #147 merged)
    - Documented hydrus/app.py (PR #154 merged)
    - Note : These were the only two scripts using Flask and relevant to my proposal (Hence chose to doument these first)
    

### My other works
- Check out https://py-ranoid.github.io/Resume

# Project Goals
## 1. Port Hydrus to Falcon (2 weeks)
### Week 1
- Fork https://github.com/HTTP-APIs/falcon-http-hydra and merge https://github.com/HTTP-APIs/hydrus into another branch (as of May 14th)
- Replace Flask's `g` with another alternative to maintain global variables in `utils.py`
- Update changes in unittests
- Convert Flask `Resource` to Falcon Resources
    - Index
    - Vocab
    - Entrypoint
### Week 2
- Convert Flask `Resource` to Falcon Resources
    - Item
    - ItemCollection
- Debug and test
- Add documentation
- Update unittests

## 2. Port Hydrus to Django (2 weeks)
### Week 3
- Fork https://github.com/HTTP-APIs/django-http-hydra and merge https://github.com/HTTP-APIs/hydrus into another branch (as of May 14th)
- Replace Flask's `g` with `settings.py`-based global variables in `utils.py`
- Update changes in unittests
- Convert Flask `Resource` to Django Generic View
    - Index
    - Vocab
    - Entrypoint
### Week 4
- Convert Flask `Resource` to Django Generic View
    - Item
    - ItemCollection
- Debug and test
- Add documentation
- Update unittests

---
---
### Week 5
- Buffer to merge Hydrus develop into the above projects
- Resolve any loopholes in the above projects
- Test and make sure the above projects are complete by the end of Week 5
- Add extensive documentation
---
---
## 3. Support Redis as Graph database (4 weeks)
### Week 6
- Establish concrete DB structure to store Hydra Items, ItemCollections, HydraDocs, etc.
- Write functions to create edges and nodes for CRUD operations
### Week 7
- Write Redisgraph Queries for CRUD operations
- Replace all SQLalchemy-based CRUD operations with Redisgraph based operation
### Week 8
- Test and Debug
- Add features based on mentor's suggestions
- TBD

## 4. Better API Querying (3 weeks)
### Week 9
- Discuss a syntax definition with mentors
- Discuss new API queries
### Week 10
- Code the CRUD part of new queries with Redis
- TBD
### Week 11
- Code the Flask part of new queries with Redis
- TBD

---
---
### Week 12
- TBD
