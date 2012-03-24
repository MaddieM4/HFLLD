# The problem that I present a solution for

If Wikipedia (and its citation of www.etymonline.com is to be believed), the term "legalese" has been in use now
since the year 1914, and the problem it describes dates back even farther. Much farther. In order to write legal
documents that are "bulletproof," one has to both be a lawyer, and write like one. From the lay point of view, this
generally means "incomprehensibly."

Now, that would be all well and good if lawyers were the only ones who had to deal with legal agreements, but that's
far from the case. Everyday citizens are put in the position of having to put their signature to massive blocks of
unreadable text, unsure how much of their life and rights they are unknowingly signing away. The same exact problem
rears its ugly head in the world of politics, where gigantic bills can be stealthily stuffed with pork, and even if
such stuffing is caught, it is often a moot point, because it's easier to simply pass the bill before it hits a
deadline. The NDAA, for example, is a recurring piece of legislation in America that does many wonderful things for
veterans, who would have lost important benefits if it was not passed on time - but the latest edition harbored a
clause that legitimized indefinite detention of United States civilians not charged with any crime. Obama signed it.
"With reservations," of course, but he signed it. While I think anyone reading this is also hoping for the judicial
branch to formally call it out for being blatantly unconstitutional, that hasn't happened yet.

And yes, it _is_ very much the same problem that is affecting us, whether it's in the form of a software EULA or a
bridge to nowhere. The problem is illegible, monstrously large legal text.

# The solution to the problem I just presented

Some might naively try to simply limit the size of legal documents. In fact, it's been tried, although such efforts
never actually get anywhere, if for no other reason than the extreme distaste that lawyers have for being forced to
work like embedded systems designers. Their job, what they are trained for, is bulletproofing. Not writing legal code
in tiny ways, not performing verbal acrobatics to compress their proper work into an equally safe minification. Their
job, which they do well, is to write obnoxiously detail-obsessed, leak-proof stuff, that will stand up to the
scrutiny of their equally obnoxiously detail-proof peers in a court of law.

No, that doesn't work for practical reasons. So, the trick is, to give the parties involved a simple version of the
agreement, give the lawyers a complex and detailed version, and make sure that the two always match up. And believe
it or not, this can be accomplished in a relatively simple way.

HFLLD's are a way of doing this, by making sure the complex stuff is present and contextually located, but hidden
from view by default. An HFLLD is composed of "pages", each of which can contain up to 5000 characters. These pages
can contain other pages between paragraphs. These subpages are clarifications of the paragraph they define, allowing
you to use clear, readable language to fully describe an agreement, and patch in details recursively as you write.
And for legal protection, no subpage may violate the intentions expressed by its paragraph, or do things outside of
its scope. If a judge rules a subpage to be misleading, it and all its descendant pages are considered invalid and
not legally binding. In other words, you can't sneak crap in.

HFLLD's provide safety, security, legibility, and foster a more collaborative process between the lawyers and the
parties involved. If a legal document defines itself as one, then all the protections apply. Any legal document,
including legislation, can be an HFLLD, simply be declaring itself as such and following the schema.

# How can I help?

The HFLLD schema and official definition is, itself, an HFLLD. If you are a lawyer, or have legal experience, you
can help expand and grow it to be more secure against fraud, loopholes, and other general assholery. 

If you are a developer, you can help work on the tools involved with the technology side, for things like recursive
muli-file composition, interactive display, conversion to PDF, etc.
