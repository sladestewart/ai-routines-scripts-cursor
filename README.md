# ai-routines-scripts-cursor
The ["AI Routines / AI Scripts"](https://github.com/sladestewart/ai-routines) concept realized in Cursor

## Notes
For Cursor, the mechanism is
- A set of three Cursor Rules that to some extent 'bootstrap up AI Routines/Scripts' for any given project
- The three Cursor Rules are:
 - ai-routines.mdc : The rules for managing AI Routines (natural-language 'scripts')
 - ai-scripts.mdc : The rules for managing (documents containing formal-language - e.g. grunt, shell, etc. - scripts but structured in a way that Cursor can use them to help with script management including execution)
 - ai-execution.mdc : Intended to contain rules governing generally, how Cursor acts on commands - from other Routines, from prompts, etc.  It currently does contain a few rules that were discovered to be helpful/necessary as these AI Routines/Scripts Cursor Rules were being developed.  NOTE: As things progress, it might make sense for this to be moved out of this repo and into some orther repo like its own dedicated repo.  We'll see.

## Implementing In Your Project
- Clone this repo.  NOTE: You almost certainly **don't** want to clone this into the project you want to use these Cursor Rules in.  You want them in a 'well-known place' and then copied into the new project - so that there's no 'git link' between this repo and your new project.
- For each new Cursor project that you want to use AI Routines / AI Scripts in, just copy these rules files (**.mdc) into the project's .cursor/rules folder

## Future Plans
Later, we'll develop a Cursor User Rule that can be 'copied to a Cursor instance' once.  Then the user will, for each project, be able to issue a command after creating the project - something like 'Terraform this project' - and things like these AI Routine Protocols will be set up in the project.  Depending on what we learn about how Cursor User Rules work - depending on that, this Cursor User Rule might be in its own repo - not sure.
