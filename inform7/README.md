# Sand-dancer by Aaron Reed and Alexei Othenin-Girard

The source files and Inform extensions for Sand-dancer, with modifications to work with the latest version of Inform from https://github.com/ganelson/inform/releases. As of September 2, 2002, this was 10.1.2 (also listed as (1.82.3).

See the 'original' tag for the sources as copied from https://inform7.textories.com/sand-dancer/

Below are the changes that were made...

My thanks to Aaron for making this freeware and encouraging further adaption of their work.

### Out-of-date Extensions

- *Conversation Framework for Sand-dancer*, by Aaron Reed
  This was some modifications on top of Eric Eve's "Conversation Framework" and "Conversation Suggestions". I've included Aaron's modifications at the end of the file.

- *Default Messages* by David Fisher
  This was used to override some common messages with more Knock likely alternatives. I've put in an example of how to do this in the current Inform but it is also true that many are handled by other extensions.
  
- *Conditional Undo* by Jesse McGrew
  This and its replacement, *Undo Output Control* by Nathanael Nerode have ceased to work with the latest version. As this was only used to stop undoing smoking, I've commented it out.
  
### Changes to Inform since last publication
- Exercise 11.4
  The syntax for `Understand the command "read about" as "consult".` has changed, you do not need `the command` and you use the name of the action (*consulting it about*) instead. That said, Inform7 now supports "read about x in book" and "Look up x in book" as synonyms so this part isn't needed (although `Understand "guide/book/page/pages" as the guidebook.` is still required to refer to it as 'book'.)
  
- Section: Radio
  - You no longer need `with parts integer and decimal`. Inform deduces this on the fly.
  - Additionally, `have the parser notice voice` is now `set pronouns from voice` .This was to allow the player to type "Tell it ..." or "Tell him ..." and it will know you mean the voice from the radio.
  - `[is-are]` is now just `[are]`
  