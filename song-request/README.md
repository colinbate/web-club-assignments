# Song Request System

## Background

So back in the day, which was sometime in early 2011, I was a bit of a KJ, or karaoke jockey. We used to have office karaoke parties on a regular basis and even hosted them in three of the other offices at different times.

I ran everything using software on my computer and karaoke files I bought or downloaded online. I started off with a decent collection of "classic" karaoke tunes, mostly Oldies. However, people often had particular songs that they wanted to sing, so in addition to a [website with schedules and announcements][oak], I built a [song request "app"][rl] which allowed people to request songs which I would try to obtain before the next show. It worked, but it wasn't great. Even by my standards at the time which means it is all utterly embarrasing now. :)

My stack at the time was:

 * Node.js
 * Express 2
 * EJS templates
 * jQuery 1.5.2
 * Hand crafted CSS
 * CouchDB

I didn't even bother to finish writing any admin interface for me to remove songs from the request list. I was using the CouchDB UI (Futon) directly to edit documents one at a time. It was tedious. And if you look at my [request list][rl] now, you can see it is full of spam which I have no easy way of getting rid of.

One things also to note is that the [list of songs][sl] on the site loads from a CSV file which I exported from my karaoke software, and is not tied to this request system. So it is easy for things to get out of sync and confusing.

[oak]: http://oakaraoke.com
[rl]: http://oakaraoke.com/request/
[sl]: http://oakaraoke.com/library/

## Assignment

Create a different/better/whatever version of this song request system using a different stack of technologies. You can reuse bits of my stack if you want, but mix it up and make it interesting. Part of the assignment is to use, for at least two parts of the stack, something which you've never used before.

### Minimum requirements

 * Create an "app" which shows a request list of songs (song name with artist) with the date requested.
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
 * Add some form of spam control: captcha, honey pot, etc.
 * Integrate this request form with a search of a pre-existing list of songs which you can populate however makes sense.
 * Allow a CSV file with songs in it to populate the song database (or be the song database).

### Notes

I'm not specifying any requirements on the UI/UX side of things, but the end result should be functional, reasonably usable and "not unattractive". Read into that double negative what you want. You **do not** have to match the style or presentation of my original app in any way.

### Inspiration

If you are looking for possible challenges with this one, consider creating this without using your own backend, rather create a static app which uses some form of backend or database as a service (aaS). Or look into [isomorphic JavaScript][iso].

[iso]: http://isomorphic.net/

