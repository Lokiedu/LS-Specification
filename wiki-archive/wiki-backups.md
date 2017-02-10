# Roadmaps

### Read / unread indication storage / architecture for every post / user.

---

### Data authoring, versioning architecture review

In this card I want to briefly touch a couple of concerns I have in regards to data architecture. I hope to invest a block of time here \(2-3 hours\) and come out with a draft plan, maybe 2-3 cards in trello for future development.

We have a vision of**knowledge authoring**concept that we'd like to discuss, and possibly, implement on LibertySoil.org

Obviously, we'd like to look at external authoring / referencing standards and best practices.

## Attribution

In it's essence it is: we want to**store attribution data for more-less each piece of "content" data that we store on LibertySoil.org**

If there's tag "Democratic Education" - we want to know who \(what LibertySoil.org user\) has authored this version of the tag "object" \(synonymous with an article in Wikipedia, their article - is our tag\).

Each new tag fields information "save" would be treated as a "version" and each version would have it's author \(user of the site\).

There should be a way to clearly and personally \(!\) attribute all main current and future site data to site users: tags \(school, hashtags, locations, posts, comments\), all additional tags data. We might arrive at "organizations" at some far future point, but at this point it's only personal level \(author = human, LibertySoil user\).

## Transparency

We'd like to not just keep this information, but with time - make it transparently visible in templates, in the API, dashboards. We'll have a "Log" page with basic history of versions, available to anyone.

All value of the site is authored by the community and all contributors are fully visible and traceable in real time.

If there's a change in authorship - previous versions are visible and rollback is possible.

Mechanics and specific features are less important now, but in the end - we will need to save each version and we will need to be able to do a rollback to a previous version.

Some data will be imported by us \(like locations\) - but even then I'd like to find a way to attribute it, where possible - maybe even with specific data references \(in case of LinkedData etc.\).

## Translations

Another thing that has to be discussed here is a language. I don't want to mix everything up in one pile, but it feels essential.

If we have "Democratic Education" hashtag, I think the text "Democratic Education" is not the tag itself. It is only the name of the tag in English. We need a way to expect tag names to be translated into other languages. Then there would be one tag with two names "Democratic Education" \(EN\) and "Демократическое образование" \(RU\), for example.

Language of the tag name does not hold any relationship with the language of the tagged posts. So "Демократическое образование" would output all posts tagged with this tag, irrespectful of name language visible to the user at the moment.

I'd like to schedule a discussion on the matter.

**p.s. Synonyms**

I don't know if this belongs here, but we have to have synonyms issue resolved somehow.

An example is plural-singular usage when we have two tags for "Democratic School" and "Democratic Schools". That's not two tags - that's one same tag. But how do we go about it with languages and versions? Is there a good way to "link" two tags together so that one tag remains, there's one page, and every "synonym" works as a redirect to that main tag \(and visible in the list of synonyms, for example\)?

This is a real problem because people get confused in multiple tags and we want to build a tool for community to condense meanings.

  


