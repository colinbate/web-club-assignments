# Song Request System

##Background

So back in the day, which was sometime in early 2011, I was a bit of a KJ, or karaoke jockey. We used to have office karaoke parties on a regular basis and even hosted them in three of the other offices at different times.

I ran everything using software on my computer and karaoke files I bought or downloaded online. I started off with a decent collection of "classic" karaoke tunes, mostly Oldies. However, people often had particular songs that they wanted to sing, so in addition to a website with schedules and announcements, I built a song request "app" which allowed people to request songs which I would try to obtain before the next show. It worked, but it wasn't very good. Even by my standards at the time which means it is all quite embarrasing now. :)

My stack at the time was:

 * Node.js
 * Express 2
 * EJS templates
 * jQuery 1.5.2
 * Hand crafted CSS
 * CouchDB

I didn't even really bother to finish writing any admin interface for me to remove songs from the request list. I was using the CouchDB UI (Futon) directly to edit documents one at a time. It was tedious.

One things also to note is that my song list of songs that I currently had was based on a CSV file which I exported from my karaoke software, and was not tied to this request system. So it was quite easy for things to get out of sync and confusing.

## Assignment

Create a different/better/whatever version of this song request system using a different stack of technologies. You can reuse bits of my stack if you want, but mix it up and make it interesting. Part of the assignment is to use for at least two parts of the stack something which you've never used before.

### Minimum requirements

 * Create an "app" which shows a request list of songs (song name with artist) with a date as to when they were requested.
 * There should be some way to create a new request which should collect:
     - Song name
     - Artist
     - User information (name and email)
 * Needs to allow an admin user to authenticate and view the list of songs
     - The requesting user info should be visible only to admins
 * Should be a way for admins to mark a request as fulfilled.
 * Fulfilled requests should still be visible to admins in another view.

### Optional work

If you are feeling particularly keen, you can try to add some of the following.

 * Allow normal (non-admin) users to sign in so they don't need to enter name or email information as part of the request form.
 * Allow normal users to see all of the songs they've requested personally and their status.
 * Admin users can sort the request list via any of the fields.
 * Integrate this request form with a search of an existing list of songs which you can populate however makes sense.
 * Allow a CSV file with songs in it to populate the song database (or be the song database).

### Notes

I'm not specifying any requirements on the UI/UX side of things, but the end result should be functional, reasonably usable and "not unattractive". Read into that double negative what you want.


