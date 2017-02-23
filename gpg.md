GPG Tutorial
============

This was once just a page that contained my public encryption key. It
has now grown to become an introduction to how and why to use the GNU
Privacy Guard encryption software (GPG) to protect your privacy. It is
continually growing. If you have questions, corrections, suggestions,
software recommendations, or want to exchange encrypted e-mails, please
contact [Alan Eliasen](mailto:eliasen@mindspring.com). I'm also on the
Twitter thingy as [aeliasen](https://twitter.com/aeliasen). Thanks!

Table of Contents
-----------------

-   [Public Key for Alan Eliasen](#PublicKey)
-   [What is Public-Key Cryptography?](#PublicKeyCrypto)
-   [What I Use](#WhatIUse)
    -   [On Android](#OnAndroid)
-   [gpg or gpg2 ?](#gpgorgpg2)
-   [Importing A Key](#ImportingAKey)
    -   [Importing from Enigmail](#ImportingFromEnigmail)
    -   [Importing from GPG](#ImportingFromEnigmail)
-   [Getting Help](#GettingHelp)
-   [Getting Started](#GettingStarted)
-   [Generating a Revocation Key](#RevocationKey)
-   [Procedure for Verification](#ProcedureForVerification)
    -   [Fingerprint](#Fingerprint)
        -   [Fingerprints in Enigmail](#FingerprintsInEnigmail)
-   [Signing a Key](#SigningAKey)
    -   [Signing Keys in Enigmail](#SigningKeysInEnigmail)
    -   [Signing Keys in GPG](#SigningKeysInGPG)
-   [Publishing your Public Key](#Publishing)
    -   [Manual Exporting](#ManualExporting)
    -   [Uploading a Public Key via GPG](#UploadingViaGPG)
    -   [Uploading a Public Key via Enigmail](#UploadingViaEnigmail)
-   [Manually Decrypting](#ManuallyDecrypting)
-   [Manually Encrypting](#ManuallyEncrypting)
    -   [Encrypting for E-mail](#EncryptingForEmail)
    -   [Encrypting Files](#EncryptingFiles)
-   [Attachments and PGP/MIME](#Attachments)
    -   [Attachments in Enigmail](#AttachmentsInEnigmail)
        -   [Disabling PGP/MIME in Enigmail](#DisablingPGPMIME)
-   [Signing Messages](#SigningMessages)
    -   [Configuring Enigmail for Automatic
        Signing](#EnigmailAutomaticSigning)
    -   [Signing a Plaintext Message](#SigningPlaintext)
    -   [Verifying Signatures](#VerifyingSignatures)
    -   [Detached Signature](#DetachedSignature)
    -   [Proving You Wrote Something but Remaining Temporarily
        Anonymous](#ProvingAnonymous)
-   [Updating Keys](#UpdatingKeys)
    -   [Updating Keys in Enigmail](#UpdatingKeysEnigmail)
    -   [Listing your Keys](#ListingKeys)
    -   [Who Signed My Key?](#WhoSigned)
-   [Building a Web of Trust](#WebOfTrust)
-   [Good Encryption Practices](#GoodPractices)
-   [Symmetric Encryption/Decryption](#Symmetric)
-   [Why Public-Key Encryption is Cool](#Cool)
-   [Tips and Tricks](#TipsAndTricks)
    -   [Using Stronger Algorithms](#StrongerAlgorithms)
    -   [Verbose Information](#VerboseInformation)
    -   [Requiring Multiple Decrypts](#MultipleDecrypts)
    -   [Hidden Recipients](#HiddenRecipients)
    -   [Encrypting Messages You Can't Decrypt](#OneWayEncryption)
        -   [In GPG](#OneWayGPG)
        -   [In Enigmail](#OneWayEnigmail)
    -   [Migrating to a New Key](#Migrating)
        -   [Creating Your Own New Key](#OwnNewKey)
        -   [Using Someone Else's New Public Key](#OthersNewKey)
    -   [Keysigning Party](#KeysigningParty)
-   [Technical Notes](#TechnicalNotes)
    -   [Short Key IDs Are Bad News](#ShortKeyID)
    -   [Finding Your Longer Key ID](#LongerKeyID)
    -   [Key IDs and Hash Algorithms](#KeyIDsHash)
    -   [Enigmail, gpg-agent, and Gnome keyring bugs](#BadGnome)
    -   [Automating GPG](#Automating)
    -   [Forcing Different Algorithms](#ForcingAlgorithms)
    -   [Protecting your Secret Keys](#ProtectingSecretKeys)
    -   [Backing Up Your Secret Key](#BackingUpYourSecretKey)
    -   ["Creating the perfect GPG keypair"](#PerfectKeypair)
    -   [OpenPGP Specification](#OpenPGPSpecification)

Public Key for Alan Eliasen
---------------------------

Below is the public encryption key for Alan Eliasen,
([eliasen@mindspring.com](mailto:eliasen@mindspring.com)) in armored
OpenPGP format. This lets you write encrypted messages that only I can
read!

**Note:** I have recently upgraded to a stronger 4096-bit RSA key. If
you were previously using the old key, please see my [key migration
document](gpgmigration.txt) for more information on the reasons for this
change and how to migrate to the new key.

Don't worry: you don't have to read this. You can cut-and-paste it or
obtain it in a [plaintext file](pgp.txt) or import it from a keyserver
using the directions in the [Importing a Key](#ImportingAKey) section of
this document.

~~~~ {.tiny}
-----BEGIN PGP PUBLIC KEY BLOCK-----
Version: GnuPG v1
Comment: See Alan's GPG guide at https://futureboy.us/pgp.html

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
pIPGkZxLOFm59msUf9mBqw7rJEs/EqhQ2w==
=7DhM
-----END PGP PUBLIC KEY BLOCK-----
  
~~~~

Fingerprint:

EC2392F2EDE74488680DA3CF5F2B4756ED873D23

Long Key ID:

5F2B4756ED873D23

Short Key ID:

ED873D23

*(Did you notice that the long and short key IDs (of any key) are just
the last 16 or 8 digits of its fingerprint respectively? I didn't know
that for a long time, but it's obvious when displayed this way. See the
[Finding your longer key ID](#LongerKeyID) section of this document for
more.)*

This is also available in a [plaintext file](pgp.txt).

What is Public-Key Cryptography?
--------------------------------

In short, public-key cryptography solves the age-old problem "how do I
communicate with someone securely without somehow exchanging a secret
password first?" Exchanging a shared password securely is a hard
problem. You may have no way to do so if your communications are
monitored.

With public-key encryption, instead of sharing a password, each party
generates a "keypair" consisting of a "public" key and a
"secret/private" key. Each party can then publish their "public" key to
the world or send it directly to the other party, while keeping their
secret key private and safe.

If you have Person B's public key, you can do a few things with it:

-   Encrypt a message that only that Person B can decrypt. (They need
    their secret key to decrypt it.)
-   Validate that Person B signed a message with their secret key. This
    also lets you verify strongly that the message was not corrupted nor
    modified in transmission.

With your secret key, you can do a few things:

-   Decrypt messages encrypted with your public key.
-   Sign messages that others can verify came from you (they need your
    public key to verify the signature.)

What I Use
----------

I accept and transmit all messages using the OpenPGP format, which is an
open standard, ([RFC 4880](http://www.ietf.org/rfc/rfc4880.txt)) and the
most widely used standard for public encryption, so communication should
work with any OpenPGP-compatible program.

For encryption and signing of e-mail (on Windows, Linux, and Mac) you
can use a combination of:

-   [GNU Privacy Guard](http://www.gnupg.org/) (GPG)
-   [Thunderbird](http://www.mozilla.org/products/thunderbird/),
    mozilla.org's stand-alone mail client.
-   The Mozilla [Enigmail](http://enigmail.mozdev.org/) add-on.

If you're on Fedora, you will have infinitely better luck installing
Enigmail from the Fedora distribution rather than obtaining the plug-in
elsewhere. Install all three packages it by doing the following as root:

`yum install gnupg thunderbird thunderbird-enigmail`

After installing or updating in Fedora, you may not see the OpenPGP
menus in Thunderbird until going to `Tools | Add-ons` and then disabling
Enigmail, restarting Thunderbird, re-enabling Enigmail, and restarting
Thunderbird.

My main gripe is that Thunderbird changes version numbers rapidly and
Enigmail sometimes doesn't keep up, which makes Enigmail claim that it's
incompatible with your Fedora version. This is an important reason to
use a package-manager like `yum` on Fedora which tends to keep them in
sync. This is another reason it's good to know how to use the gpg
executable manually.

The first thing you want to do in Enigmail is to make all of its
settings visible. You can do this from the menu items
`Enigmail | Preferences |       Display Expert Settings and Menus`. The
basic settings are inadequate.

**Note:** As of the latest update of Enigmail, around July 2014, the
text used in several menu items has changed. The old top-level menu item
was called `OpenPGP` and the new one is called `Enigmail`. You may need
to mentally correct these examples if you're using an old version of
Enigmail.

In Enigmail, I've had the best luck setting the keyserver to default to
`pgp.mit.edu`{.input}, but this may no longer be necessary as it now
contains a list of default keyservers which are more stable than they
used to be. (But often still down.)

The Gnu Privacy Guard
[FAQ](http://www.gnupg.org/faq/GnuPG-FAQ.html#which-email-client-can-i-use-with-gnupg)
lists some of the other e-mail programs compatible with GPG. Note that
you can use *any* e-mail program (that doesn't corrupt messages) along
with the `gpg` executable on the command-line.

For Macintosh, you can obtain GPG from the
[GPGTools](https://gpgtools.org/) website. (I haven't personally used
these, but others have recommended them.)

Alternately, I sometimes use the `pgg` package in Emacs/XEmacs which is
a wrapper around the `gpg` executable's functions. You can do something
like highlight a region and do: `M-x pgg-encrypt-region` and encrypt
directly within your documents.

For encrypting files, or doing anything more interesting, I just use the
`gpg` program on the command-line. If you're security-paranoid, the
fewer executables, the better. Most of this document teaches you the fun
and important things you can do with the `gpg` program to be secure.

### On Android

On Android, you may want to experiment with
[R2Mail2](http://r2mail2.com/). I haven't used it and can't vouch for
it. There is also [Android Privacy Guard
(APG)](https://play.google.com/store/apps/details?id=org.thialfihar.android.apg&hl=en),
which integrates with the [K-9
Mail](https://play.google.com/store/apps/details?id=com.fsck.k9&hl=en)
program, but I do not vouch for it. APG was not updated for a few years,
but has seen activity more recently.

gpg or gpg2 ?
-------------

GPG version 2 may be on your system with the executable name `gpg2` .
Either executable can be used for these demonstrations. Both are very
compatible with each other. (If you want to know a million different
opinions on which you should be using, do a web search.) Version 1 is
more tested, and is usually a single monolithic executable. Version 2 is
compiled with crypto libraries like `libgcrypt` externally linked, and
is designed to work better with external password entry tools. That is,
`gpg2` is designed for graphical environments, while `gpg` works better
for automated and command-line use. From the command-line, I use version
1.

**Update October 2015:** I have now seen cases where `gpg` cannot import
keys from some clients, notably keys sent by
[Mailvelope](https://www.mailvelope.com/) (link opens in new window,) a
client that helps you use encryption with web-based e-mail services like
GMail or Yahoo. When importing the key, the error message may look
something like:

`gpg: assuming bad signature from key BACD0190 due to an unknown critical bit gpg: key BACD0190: no valid user IDs     gpg: this may be caused by a missing self-signature    `

In this case, the `gpg` executable is telling you that it doesn't
understand some of the subpackets sent in the message, and, according to
the [OpenPGP specification, (RFC 4880 Section
5.2.3.1)](https://tools.ietf.org/html/rfc4880#section-5.2.3.1), `gpg` is
correct in treating the signature as invalid if it doesn't understand
the subpacket type:

> 'Bit 7 of the subpacket type is the "critical" bit. If set, it denotes
> that the subpacket is one that is critical for the evaluator of the
> signature to recognize. If a subpacket is encountered that is marked
> critical but is unknown to the evaluating software, the evaluator
> SHOULD consider the signature to be in error.'
>
> 'An evaluator may "recognize" a subpacket, but not implement it. The
> purpose of the critical bit is to allow the signer to tell an
> evaluator that it would prefer a new, unknown feature to generate an
> error [rather] than be ignored.'

If you encounter this case, then `gpg` likely did *not* import the
public key correctly, and you will need to try to use `gpg2` to import
the public key. (For me, `gpg2` could import public keys that `gpg`
could not.) It appears that, once you have correctly imported the public
key, you may be able to use `gpg` or `gpg2` to communicate with the
other party, depending on the particular feature that was requested.

By the way, at this point, I neither endorse nor discourage use of
Mailvelope. I have used it to apparently encrypt communications
correctly with GMail users, though.

Importing A Key
---------------

### Importing From Enigmail

The simplest way to import my key from an e-mail client (like Enigmail)
is to import it from a keyserver. In Enigmail, you can search for keys
using the menu items
`Enigmail | Key Management | Keyserver | Search for     Keys`, and then
searching for my name or my e-mail address `eliasen@mindspring.com` or
my key ID, which is `5F2B4756ED873D23` or the shorter `ED873D23`. Then
select its checkbox from the list and click "OK."

A lazier and more dangerous way to import my public key from Enigmail is
to try and send me an encrypted e-mail. (When composing a message,
choose the menu item `Enigmail` and select both `Sign     Message` and
`Encrypt message`.) Then, when you try to send, Enigmail will realize
that it doesn't have my public key, and will bring up the Key Management
window. From there, you can choose `Download Missing Keys`.

Another way to import my key is to e-mail [the plaintext version of my
key](pgp.txt) to your own e-mail address and choose the option like
"Import PGP Key."

### Importing From GPG

If your e-mail client doesn't allow automatic import of keys from an
e-mail message, you will need to save the plaintext file listed above
key to a file, then import the key manually. From GNU Privacy Guard,
this is:

`gpg --import [filename]`

My key is available from `pgp.mit.edu` (all the major keyservers mirror
each other, so you could probably get it from the keyserver of your
choice, but this one seems to be pretty reliable.)

You can browse the keys available on keyservers at
[pgp.mit.edu](http://pgp.mit.edu/) or the often-slow
[sks-keyservers.net](https://sks-keyservers.net/). Who do you know who
has a posted public key?

From GNU Privacy Guard, you could import my key using the following (but
read on to be more secure.)

`gpg --keyserver pgp.mit.edu --search-keys eliasen@mindspring.com`

Note that in all of these examples, whenever you see an e-mail address,
you can usually substitute part of a name or part of an e-mail address,
or a key ID. Most of these commands perform a substring search.

Or, even more directly, my full key fingerprint is
`EC2392F2EDE74488680DA3CF5F2B4756ED873D23`, (it's more common but less
secure to use the last 16 or 8 characters of a key, so `ED873D23` will
work too. (Note that the shorter key IDs are just the last 16 or 8
characters of the fingerprint!) Read the technical note on [Short Key
IDs](#ShortKeyID) below for interesting attack ideas using short keys.)
The following gpg command will import my key from a keyserver, using my
full fingerprint (you can also use the last 8 or 16 hexadecimal digits
of the fingerprint as the short or long key IDs.)

`gpg --keyserver pgp.mit.edu --recv-keys EC2392F2EDE74488680DA3CF5F2B4756ED873D23`

Read on, though, and see why just importing some key off a keyserver
isn't enough to be sure that you're talking with *me*.

You may not have to specify a keyserver in the lines above. Later
versions of GPG have a more reliable keyserver list built in.

[sks-keyservers.net](http://sks-keyservers.net/status/) monitors the
status of keyservers in real-time. (But it's often down.) If you're
having trouble importing signatures from a specific keyserver, or want a
list of available keyservers, you might want to look there.

Getting Help
------------

`gpg --help`

is your friend. It will list the most common options to GPG (but not all
of them.) Other complete documents are available:

-   [GPG Manual](http://www.gnupg.org/documentation/manuals.en.html)
-   [Using the GNU Privacy
    Guard](http://www.gnupg.org/documentation/manuals/gnupg/)
-   [The GNU Privacy Handbook](http://www.gnupg.org/gph/en/manual.html)

Getting Started
---------------

I long resisted the temptation to give an overly-simplified "Getting
Started" section here because that may falsely lead you to believe that
you're being secure. As this document has expanded greatly, it's
becoming a better guide. However, the best way to get started with
encryption is to go to the home site for [GNU Privacy
Guard](http://www.gnupg.org/) and read the "GNU Privacy Handbook"
(available in lots of formats and languages) under the "Guides" section.
This will walk you through setting up GPG on your system, including
creating your secret keys.

Creating your secret key will start with:

`gpg --gen-key`

You should probably use the default settings, except it doesn't hurt to
make the key size as large as allowed (4096 bits currently.) The larger
the key size, the longer it will take to initially generate your key
(and encryption/decryption will be slightly slower. That is a Good
Thing, as anyone attempting to break your encryption will also need to
spend more time too.)

Generating a Revocation Key
---------------------------

After generating your key, one of the first things you should do is
create a revocation certificate:

`gpg --gen-revoke --armor --output=RevocationCertificate.asc your@email.address`

This certificate can be used to revoke your key if it is ever lost or
compromised. *Do not neglect this step!* Print it out, save it on a
disk, and store it safely. It will be short enough that you can type it
back in by hand without much effort if you just print it out.

If you lose your secret key or it is compromised, you will want to
revoke your key by uploading the revocation certificate to a public
keyserver (assuming you uploaded your public key to a public keyserver
in the first place. See below.)

If you have multiple unrevoked public keys and you have messages that
say something like "I lost that one, this new key supersedes the other
ones," (and I've seen this from people who like to claim crypto
experience) then I know *instantly* that I can't trust you to follow
good practice and maintain your secret information, and that I shouldn't
trust you with my secrets. So protect your revocation key like you
protect your secret keys. Read on to see why the "this key is my new
key, ignore the others" excuse is an immediate "red flag" that should
make you suspect either cryptographical incompetence or warn you that
the person's being impersonated.

Using Stronger Algorithms
-------------------------

This section is optional but important.

By default, gpg uses weaker encryption algorithms than it could. This is
to ensure compatibility with older versions.

If you want to start using stronger algorithms from the beginning, jump
to the [Using Stronger Algorithms](#StrongerAlgorithms) section below to
see how to use stronger algorithms by default. It may be important to do
this from the start, as the algorithms that you want to use are
specified in your public key. (To be more specific, your public key
lists the algorithms that you request *other people* to use when they
encrypt messages to you.)

Procedure for Verification
--------------------------

Now, since you have my public key, are we secure? Well, no, not at all.
Lots of people just getting started with cryptography don't realize that
they have to somehow *verify* that this key belongs to me. To me, Alan
Eliasen. The one who wrote this message. How do you know that the public
key posted above is the one I posted? After all, the bad guys could have
replaced it somehow.

Listen carefully. This is important. *Anyone* can generate a public key
for *any* e-mail address. *Anyone* can post that key to *any* key
server. *Only by verifying that the key really belongs to the person you
think it does does it give you any security.* Without this crucial
verification, all that your cryptographic software does is ensures that
bits weren't corrupted during transmission, and prevents casual
observers from reading the message. It does *not* mean that you're
talking to who you think you are. You could be talking to someone else
entirely (a bad guy,) or you could be subject to a man-in-the-middle
attack.

**Update:** As proof of the above paragraph, after I posted this
document widely, on 2013-07-12, somebody generated a fake public key
with my e-mail address and uploaded it to a key server! *This is why you
need to validate the key directly with the person to make sure you have
the right key and the right person!* That is, however, an unavoidable
problem with public key servers. I thus can't be mad about it, but I
*can* try to educate people to recognize this possibility and do the
right thing by validating my public key with me personally! Note that
picking a key from multiple options on a keyserver based on which is
newest or largest or by comments about "this is my newest key" *is
dangerous and wrong.*

Still, if you want to send me encrypted e-mail, that may prevent other
people from reading it. That's good, and sometimes that's all you need.
Just understand why I don't have any reason to trust that you're who you
say you are, and you don't have any reason to trust that you're really
talking to *me* unless you've verified my key with me. Before I trust
you with any secrets, I'll validate your identity.

### Fingerprint

A key could be verified in many ways (such as, I could read you my whole
public key, which is really time-consuming and error-prone. It's also
bad because the key you see above can get longer and longer as other
people sign it.) The usual alternative is to compare the *fingerprint*
of what *you* think my public key is with the fingerprint of what I
*know* my public key is.

A fingerprint is a shorter number (usually expressed as a
40-hexadecimal-digit number) that contains a cryptographically strong
hash of my public key. It's shorter than my full key, so it's not an
unfoolable test, but the probability of finding another key with this
fingerprint is very small indeed. Infinitesimally small. So small you
don't have to worry about it. If someone else can find a matching
fingerprint, they have enough power and money that they could make you
vanish from the face of the earth. So, after you've imported my key,
type:

`gpg --fingerprint eliasen@mindspring.com`

This will produce output that looks something like below (I have put the
fingerprint in bold.)

` pub   4096R/ED873D23 2014-07-22       Key fingerprint = EC23 92F2 EDE7 4488 680D  A3CF 5F2B 4756 ED87 3D23 uid                  Alan Eliasen <eliasen@mindspring.com> sub   4096R/5314E70B 2014-07-22    `

Then, you need to verify this fingerprint with me. It's best to do it
face-to-face, but if it's someone you know by voice, you can do it on
the phone. If you don't know the person, check their driver's license.
Ask other people (that you trust) who know them. Even if you don't know
them, at least you're verifying that the key belongs to the person
you're talking to.

The other person will need to verify that their (unverified) copy of
your public key matches what you know your public key to be. So bring a
copy of your own fingerprint to the exchange:

`gpg --fingerprint your@email.address`

Of course, change the e-mail address above to the e-mail address you're
confirming.

*Corollary:* If someone puts the fingerprint of their key in their
e-mail signature, or in a web page, they really aren't proving their
identity. Think about it. If someone's pretending to be you, and forging
your e-mail or your web site, they'd certainly replace the fingerprint
too. It's not enough to rely on. If you see someone with their key
fingerprint in their e-mail signature, it's not a reliable sign that the
key with that fingerprint truly belongs to them.

#### Fingerprints in Enigmail

If you want to view a person's fingerprint or key ID in Enigmail, you
can view that in the "Key Management" dialog, which is the place where
you can view and manage public and private keys for everyone in your
keyring.

The steps to view the fingerprint are to follow the menu items:
`Enigmail` | `Key Management` | Search for a name | Right-click the name
| `Key Properties`. This will bring up a dialog containing lots of
information about the key, including its key ID and fingerprint
(unfortunately, it's not easily printable.)

### My Key Verification Protocol

If you wish to verify this key, please contact me and I will verify its
fingerprint in a public meeting-place. I will be wearing a trenchcoat
and a navy blue ascot. You must wear or carry a yellow tulip. Any other
flower signifies that contact should be aborted, even if the exchange
below is executed correctly. I must not underestimate the necessity of
having an adequate stock of proper yellow tulips on hand for this
purpose.

I will say "The adobe is filled with an excess of straw this season."

You must reply "The straw is for the young lambs which roam the heaths
near Glasgow in the green, green spring."

If I am satisfied with your response, I will reply "The greens at Saint
Andrew's are boiled with ham and contain an excess of bitter kale."

Do not make eye contact or show signs of recognition. If necessary, I
will read the hexadecimal digits of the fingerprint while feigning a
book order on my cell phone.

Okay, I'm sort of kidding about this section. But you *must verify keys
with the other person to be truly secure.*

If you have verified my key, and trust me (and trust your own
verification,) be sure to sign it.

Signing a Key
-------------

Now that you've verified my identity, and my public key, you need to
tell your cryptographical software that you trust my key. Otherwise,
your cryptographical software should do the right thing and warn you
that you're communicating with someone that you haven't verified. It's
telling you that it has no reason to believe that the key you're using
is the one that actually belongs to that person.

Below are tips for signing and trusting keys using both GPG and
Enigmail.

### Signing Keys in Enigmail

I'm a bit reticent to recommend using Enigmail to sign keys because some
of its dialogs are deceptive and wrong. Read the next part very
carefully.

In Enigmail, you can sign keys by going to the menu item
`Enigmail | Key Management`.

Search for the key, and then right-click it. You'll get the option to
sign the key.

After signing the key, you should assign a trust level to the *person*
signing the key. Right-click the key name and choose "Set Owner Trust".
**Warning:** This currently pops up a dialog that asks "how much do you
trust the key?" but that's *not the right question*! The meaning of
trust in the GPG software is *how much you trust the **person** to
validate **other** people's keys*, not how much you trust the key
itself! In GPG, the question is stated as:

> "Please decide how far you trust this user to correctly verify other
> users' keys (by looking at passports, checking fingerprints from
> different sources, etc.)"

As you can see, that's a totally different question. This is why I
encourage you to learn by using GPG on the command-line. It tends to be
more rigorous and correct. Also GPG gives you more warnings about
selecting dangerous choices like "trust ultimately." Read the next
section to find out more.

### Signing keys in GPG

To sign my key from gpg, you'll do something like:

`gpg --sign-key eliasen@mindspring.com`

(but see below for a better option.)

This will give you some options for signing the key. Even better would
be to edit your signature *and* trust settings for this user using the
interactive menu:

`gpg --interactive --edit-key eliasen@mindspring.com`

*Hint:* Type `help` for the interactive commands. The commands `sign`
and `trust` are the ones you're looking for. These allow you to both
sign a key and indicate how much you trust me to verify *other* peoples'
keys. If you think I'm stupid and lax when verifying and signing other
peoples' keys, you'd assign me a low trust rating.

After you've signed someone's key, you should send it back to them so
they can show other people that you've signed it. You can export their
key using:

`gpg --export --armor their@email.address`

and then sending that output to them. They can then import the changes
using

`gpg --import`

In Enigmail, you can also attach any of the public keys in your keyring
to an e-mail. As you're composing the email, select
`Enigmail | Attach     Public Key...` and select the e-mail addresses to
attach. Note that these will not show up in the body of the message, but
as a (possibly-encrypted) attachment, possibly using PGP/MIME. For
maximum portability, I recommend attaching using the `--export` method
above and including the public key in the body of the message. My
reasons are stated in the [Attachments](#Attachments) section.

You can also upload that signature to a keyserver, which makes that
signature available to the world. See the [Publishing your Public
Key](#Publishing) section below for how to do this.

If you're really not sure about my identity, and don't want to vouch for
me publicly, you can *locally* sign my key, which means that you trust
it for your own use only:

`gpg --lsign-key eliasen@mindspring.com`

*Hint:* If you publicly sign my key without actually verifying it with
me, I'm going to assign you a very low trust rating.

Publishing your Public Key
--------------------------

Sure, you can manually send your public key to people you want to
communicate with, but what if someone needs to communicate with you
securely and you haven't sent them your public key? The usual way is
that you publish your public key to a keyserver so that anyone can
import your key. Most of the keyservers in the world mirror each other,
so a short time after you have posted your key to one server, it will be
propagated to the others. As I have said above, I've had good luck for
the past decade with `pgp.mit.edu`.

You have some responsibilities before publishing your public key (or
someone else's) to a keyserver, though. As mentioned above in the
[Getting Started](#GettingStarted) and [Procedure for
Verification](#ProcedureForVerification) sections, you better have
generated a revocation certificate for your key and put it somewhere
very safe. Otherwise, if you lose your secret key, or it becomes
compromised, the corresponding public key will sit *forever* on public
keyservers, mocking you and demonstrating that you don't know how to
protect your secrets properly. If you think you can delete a key from a
keyserver, rather than revoking it, read the [FAQ at MIT's
keyserver.](http://pgp.mit.edu/faq.html) (I think it's funny and awesome
that they have a fake "delete a key" field on their website that just
redirects to that FAQ no matter what key you enter.)

If someone has your public key, they can basically do a few things with
it:

1.  Encrypt messages that only you can decrypt.
2.  Validate that messages were signed by your secret key with a strong
    guarantee of certainty, and ensure that those messages were not
    tampered with or corrupted in transmission.

These are good things. You *want* people to have your public key. So
below are a few methods of publishing your public key to a keyserver.
All achieve the same results.

### Manual Exporting and Uploading

Now that you have generated a secret key and a public key, how do people
find your public key so that they can send encrypted mail to you? You
can send someone your public key directly by, say, putting it in an
email. To generate a copy of your public key that is easily e-mailed,
you can do:

`gpg --armor --export your@email.address`

This will generate a nicely-formatted "ASCII armored" version of your
public key which is suitable for e-mailing. "ASCII armor" is just a way
of turning raw binary data (which will probably get corrupted if you try
to send it through most e-mail programs) into a format using only
limited ASCII characters, line-wrapped, with appropriate headers, and
suitable for e-mailing. (Hint: It'll look something like my public key
at the top of the page.)

Note that the lines that begin

`-----BEGIN PGP PUBLIC KEY BLOCK-----`

and end with

`-----END PGP PUBLIC KEY BLOCK-----`

*are* a necessary part of the message. Don't forget to include them!

Once you have this ASCII-armored public key, you can manually paste it
into a form at a public key server like
[pgp.mit.edu](http://pgp.mit.edu/)

Again, just because someone seems to have sent you their public key,
there's no reason to trust that it's from that person unless you have
validated it with them using the instructions in the [Procedure for
Verification](#ProcedureForVerification) section above. Make sure you
verify any keys before trusting them!

### Uploading a Public Key via GPG

One way to publish your key to a keyserver is the manual approach from
the previous section: export an ASCII-armored key and manually paste it
in to a form like the one at [pgp.mit.edu](http://pgp.mit.edu/).

The other way is to let your `gpg` program upload the key. You can't do
this by specifying the e-mail address; you need to specify the public
key's hexadecimal ID number. So how do you find this for the key you
want to upload?

`gpg --list-keys your@email.address`{.input}\
\

` pub   4096R/ED873D23 2014-07-22 uid                  Alan Eliasen <eliasen@mindspring.com< sub   4096R/5314E70B 2014-07-22    `{.output}

In the above, my public key id is displayed on a line that says `pub`
and contains an 8-character hexadecimal code (`ED873D23` in the sample
above.) You will need to know this code to upload to the server.

`gpg --send-keys keyID`{.input}\
 `gpg: sending key ED873D23 to hkp server subkeys.pgp.net`{.output}

You may want/need to insert `--keyserver pgp.mit.edu` as options to the
above if you want a specific keyserver. (These options have to go
*before* commands like `--send-keys`. Again, most keyservers mirror each
other, but it will take time for keys to propagate across all servers.

Note that after you've signed *someone else's* public key, indicating
that you've verified their key and identity and vouch that the key is
theirs, you can use this same procedure to upload your signed version of
their public key to a keyserver, so people can see you've vouched for
them. See the [Web of Trust](#WebOfTrust) section below for more
information about this.

### Uploading a Public Key via Enigmail

Again, in Enigmail, everything you do with keys is accessed through the
menu item `Enigmail | Key Management`. Search for the key you want to
upload, right-click it, and you have the option to upload it to a
keyserver. Couldn't be easier! You still have the same responsibilities
to be very careful with signing other people's keys, though.

Manually Decrypting
-------------------

So you've received a file or message encrypted with GPG, but you don't
have a fancy e-mail plugin to help you decode it. So how do you decode
manually? Simple. From the command-line, if you just run `gpg` it will
prompt you for input:

`gpg`{.input}\
 `gpg: Go ahead and type your message ...`{.output}

From there, you can just cut-and-paste your message directly into gpg,
and it will decrypt it, or import keys, or whatever is appropriate to
the message. When you're done pasting, you may need to send your
operating system's "end-of-file" character. This is `Ctrl-D` in most
Unixlike systems and `Ctrl-Z` in Windows-like systems.

If the encrypted data is in a file, you can automatically process it by
just passing the filename to gpg on the command-line.

`gpg myfilename`{.input}\

The gpg executable will generally just do the right thing with it,
prompting you for passwords when necessary, saving output files, etc.

**Warning:** When gpg encrypts or decrypts a file, it usually *leaves
the original file intact!*. You must remember to delete the original
file yourself, securely if possible. In Linux, you can use `shred -u`
(shred just overwrites by default; the `-u` is necessary to delete the
file afterward) or `wipe` commands to delete securely. On Windows,
[sdelete](http://technet.microsoft.com/en-us/sysinternals/bb897443.aspx)
works well. (Although secure deleting isn't guaranteed to work on solid
state drives or flash drives due to wear-leveling algorithms. If you're
using one of these, and want to securely delete, you have to write over
*all your free space* with a tool like `wipe` or `sdelete`) However,
don't believe the hype that you need to do dozens of overwrite steps.
[This is very likely urban legend, or marketing
lies.](http://www.nber.org/sys-admin/overwritten-data-gutmann.html) One
overwrite is probably plenty.

Manually Encrypting
-------------------

### Encrypting for E-mail

If you don't have a fancy e-mail plugin that helps you encrypt your
messages, it's easy enough to do from the command line. You'll need to
save your message to a file.

`gpg --encrypt --sign --armor -r recipient@email -r     your@email.com filename`{.input}

There are several important things in this command.

-   `--encrypt` tells gpg to encrypt the message using public-key
    encryption.
-   `--sign` adds a digital signature that lets you guarantee that the
    message was generated by you and was not corrupted nor modified in
    transmission. This is theoretically optional, but see the [Signing
    Messages](#SigningMessages) section below for why this is very
    important.
-   `--armor` wraps your output in plaintext "ASCII armor". "ASCII
    armor" is just a way of turning raw binary data (which will probably
    get corrupted if you try to send it through most e-mail programs)
    into a format using only limited ASCII characters, line-wrapped,
    with appropriate headers, and suitable for e-mailing. This is
    necessary if you're pasting this into the body of an e-mail, or
    usenet posting, or forum posting, etc.
-   `-r recipient` Specifies recipients of the message. You must already
    have imported the public keys of the recipients. You can specify
    multiple recipients. If you don't specify recipients on the
    command-line, gpg will prompt you to enter them interactively. These
    recipients can also be key IDs.

    **Warning! This is important and interesting!** Note that in the
    example above, *your* email address is specified as one of the
    recipients. If you do not explicitly add *your own* address to the
    list of recipients, *you will not be able to decrypt the message!*
    That is interesting and important and awesome. You may want to write
    something and send it to someone *that you cannot ever possibly be
    compelled to decrypt!* It will be impossible for you to decrypt,
    even though you wrote it and encrypted it! That is cool. Read the
    [Why Public-Key Encryption is Cool](#Cool) section below for more
    about why public-key encryption is cool.

-   `filename` is the filename of the file you're encrypting. This is
    not strictly required. If you don't specify a filename, GPG will
    listen for input, and you can type a message directly or cut and
    paste it in. This is awkward, though. When you're done pasting, you
    may need to send your operating system's "end-of-file" character.
    This is `Ctrl-D` in most Unixlike systems and `Ctrl-Z` in
    Windows-like systems.

    **Warning:** (I'm repeating this again.) When gpg encrypts or
    decrypts a file, it usually *leaves the original file intact!*. You
    must remember to delete the original file yourself, securely if
    possible. See the [warning above](#Shred) for more details on how to
    do this.

### Cifrare dei documenti

GPG non funziona solo con le e-pistole! Volendo, puoi usarlo anche per proteggere i tuoi documenti importanti. Encrypting your files is just about like
encrypting an e-mail. The simplest command line is:

`gpg --encrypt filename`{.input}

This will prompt you for the recipients (which should include your own
e-mail address so you can decrypt it!)

A more complete command-line might look like:

`gpg --encrypt --sign -r your@email.com filename`{.input}

Some interesting things to note and optional arguments:

-   `--encrypt` tells gpg to encrypt the message using public-key
    encryption. (See the [Symmetric Encryption/Decryption](#Symmetric)
    section below for alternate ways to encrypt a file with a simple
    password and no public keys.)
-   `--sign` adds a digital signature that lets you guarantee that the
    message was generated by you and was not corrupted nor modified in
    transmission. This is theoretically optional, but very important.

    Think about it: how do you know that someone didn't replace your
    encrypted file with a different one? By digitally signing the
    message, you can get a strong guarantee that you're the one who
    encrypted the message and that it hasn't been tampered with or
    corrupted. See [Signing Messages](#SigningMessages) section below
    for more on digital signatures.

-   `--armor` (optional, probably unnecessary) wraps your output in
    plaintext "ASCII armor". "ASCII armor" is just a way of turning raw
    binary data (which will probably get corrupted if you try to send it
    through most e-mail programs) into a format using only limited ASCII
    characters, line-wrapped, with appropriate headers, and suitable for
    e-mailing. This is necessary if you're pasting this into the body of
    an e-mail, or usenet posting, or forum posting, etc. Note that this
    will increase the size of your message on disk.
-   `--output filename` (optional) specify the output file.
-   `-r recipient` Specifies recipients of the message. Can also be
    written `--recipient`. You must already have imported the public
    keys of the recipients. You can specify multiple recipients with
    multiple `-r` arguments. If you don't specify recipients on the
    command-line, gpg will prompt you to enter them interactively. These
    recipients can also be key IDs.

    **Warning! This is important and interesting!** Note that in the
    example above, *your* email address is specified as one of the
    recipients. If you do not explicitly add *your own* address to the
    list of recipients, *you will not be able to decrypt the file!* That
    is interesting and important and awesome. You may want to create a
    file for another person *that you cannot ever possibly be compelled
    to decrypt!* It will be impossible for you to decrypt, even though
    you wrote it and encrypted it! That is cool. Read the [Why
    Public-Key Encryption is Cool](#Cool) section below for more about
    why public-key encryption is cool.

-   `filename` is the filename of the file you're encrypting. This is
    not strictly required. If you don't specify a filename, GPG will
    listen for input, and you can type a message directly or cut and
    paste it in. This is awkward, though. When you're done pasting, you
    may need to send your operating system's "end-of-file" character.
    This is `Ctrl-D` in most Unixlike systems and `Ctrl-Z` in
    Windows-like systems.

    **Warning:** (I'm repeating this again.) When gpg encrypts or
    decrypts a file, it usually *leaves the original file intact!*. You
    must remember to delete the original file yourself, securely if
    possible. See the [warning above](#Shred) for more details on how to
    do this.

Attachments and PGP/MIME
------------------------

What do you do if you want to send an encrypted file attachment in an
e-mail?

There is a standard called PGP/MIME that try to standardize the handling
of encrypted attchments. You cannot be sure that your recipient's e-mail
client will be able to handle them, so I strongly recommend *never using
them*. Enigmail doesn't even handle its *own* attachments that it
creates well.

Examples of situations that will cause PGP/MIME or S/MIME attachments to
fail or be lost:

-   Most web-based email services.
-   Most phone- and tablet-based email software.
-   List servers or remailers that strip attachments.
-   List servers that just don't handle all attachments perfectly.
-   Corporate firewalls that remove attachments.
-   Overeager malware scanners.
-   Simple, secure e-mail clients that can only display plaintext.
-   Not-yet-ready-for-attachments e-mail tools like Enigmail itself.

I strongly recommend *always* sending encrypted messages or encrypted
attachments as ASCII-armored OpenPGP blocks directly in the body of an
e-mail. This will ensure that any e-mail program will still be able to
handle them.

You can hand-encrypt any attachments using:

`gpg --armor --encrypt --sign -r your@email.com     -r recipient@email.com filename`{.input}

as outlined in the [Encrypting Files](#EncryptingFiles) section above.
Then just paste the results into the body of your e-mail. You can paste
in multiple attachments this way, too.

### Attachments in Enigmail

Enigmail is buggy and insecure when sending and receiving encrypted
attachments or PGP/MIME. *I don't recommend it at the moment. In fact,
the bugs are so severe that Enigmail's behavior may allow others to
obtain your entire secret key.*

Enigmail fails, for instance, to import a public key or other
attachments that it attached itself. You can test this by sending
encrypted attachments and public keys to yourself.

Enigmail is also insecure in handling PGP/MIME (and possibly S/MIME)
attachments because it appears to always automatically and silently
decrypt the message for you, *even if you have Enigmail configured to
not decrypt by default!* This is very bad if someone's looking over your
shoulder, or detecting emanations from your monitor (e.g TEMPEST) or
doing [sound-based attacks](http://www.tau.ac.il/~tromer/acoustic/). You
may not even notice that the message was encrypted, and forget to
encrypt your reply, or forget to verify the signature, or do something
that compromises your security. It turns out that this is a known bug
[Enigmail Bug \#226](http://sourceforge.net/p/enigmail/bugs/226/) which
the developers have inexplicably labeled as "Minor." Augh. They are
obviously oblivious to the literature. In fact, the *creators* of the
RSA algorithm have explicitly stated in one of the most
widely-circulated papers on GPG that this particular bug in Enigmail is
what lets them completely steal your private key, using nothing but a
microphone near your computer or an electrical connection (e.g. touching
your skin or monitoring your computer's electricity usage) while you
receive an e-mail!

Even if you fix the problem above, Enigmail is *still* buggy when
handling PGP/MIME messages, as it will try to auto-save your messages as
you write them, which can pop up a dialog asking you to choose
recipients to encrypt to while you're typing, causing you to randomly
select recipients as you type. It's just totally broken and annoying.

For these reasons, I recommend using the manual procedure above, but
here are some tips for using Enigmail if you're lazy and don't care if
your attachments get lost or are unreadable by your recipient.

#### Disabling PGP/MIME in Enigmail

The place to turn off PGP/MIME in Thunderbird/Enigmail has been
continually changing, but now it's currently hidden under each e-mail
account on the (usually) left-hand side of your screen under
`OpenPGP Security` where the option `Use PGP/MIME by default` should be
unchecked. Here's the [current screenshot from the Enigmail
project](https://www.enigmail.net/documentation/per-account.php) showing
where PGP/MIME should be turned off for each account.

When sending encrypted e-mails with attachments in Enigmail, you will be
presented with a dialog asking how you want files to be attached:

![Enigmail file attachment prompt. Choose the option for using inline
PGP.](images/smime.png)

Choose the option "Encrypt/sign each attachment separately and send the
message using inline PGP." However, this doesn't even do the right
thing. Its results are unfortunately *not* identical to the recommended
"hand-encrypt and paste" technique described above. It currently still
adds multiple attachments, which may get stripped out by mail filters or
lost in web-based e-mail clients. Enigmail is then often unable to open
these attachments reliably. It certainly can't open public keys that it
attaches. Really, just don't use Enigmail for attachments right now.
Hand-encrypt them as shown in the previous section. It'll simply work
better for more people.

In short, all encrypted communications will be accessible to the most
people if you always just use ASCII-armored OpenPGP blocks in the body
of a plaintext message.

Signing Messages
----------------

In addition to encryption, gpg allows you to digitally "sign" messages,
which has multiple benefits:

-   It lets you ensure that a message has not been corrupted nor
    modified in transmission.
-   It allows someone to verify that *you* signed it. (To be more
    precise, to verify that the signer of the message used your secret
    key, given that they've verified your public key with you, and that
    your secret key hasn't been compromised.)

You should always sign your encrypted messages. Think about it.
*Everyone* potentially has your public key. That's expected. *Anyone*
can encrypt a message to you using your public key, and pretend that
it's from someone you know. (It's easy to spoof e-mails, but that's
another discussion.) *Only if you verify (via the digital signature)
that the message was signed by someone whose key you have verified, can
you trust the communication.*

*Corollary:* You should actively distrust unsigned encrypted
communications. If someone's trying to impersonate your friends, they'll
just conveniently "forget" to sign their messages.

A signed message gives a mathematically *very* strong certainty that the
message was signed by you.

In your e-mail client, always choose to sign *and* encrypt a message.
Below are some ways to sign messages manually.

### Configuring Enigmail for Automatic Signing

By default, Enigmail does *not* automatically sign encrypted e-mails.
This is a bad choice, in my opinion (stated in the section above.)

You can, however, make Enigmail automatically sign all encrypted mails.
The setting is *very* hard to find, though. You need to do the
following:

-   The first thing you want to do in Enigmail is to make all of its
    settings visible. If you haven't done so already, you can do this
    from the menu items
    `Enigmail | Preferences | Display Expert Settings`. The basic
    settings are inadequate.
-   Start to compose a new e-mail. That is, click the "Write" button.
-   In the "Write" window, choose the *top* menubar item
    `Enigmail | Default Composition Options | Signing/Encryption      Options`.
-   Check the `Sign encrypted messages by default` box.
-   Click OK.

### Signing a Plaintext Message

Sometimes you just want to sign an unencrypted message to make it clear
that you produced it and that it hasn't been tampered with nor corrupted
in transmission. For example:

-   Sending an important vote.
-   Important business communications.
-   Maybe you're mailing a URL that looks suspicious and spammy, and
    your recipient wants to validate that it's actually from you and not
    from a spammer or a virus. (Saying "this is really from me" in the
    e-mail is not good enough!)
-   Being very certain that the message is not corrupted in
    transmission.
-   Allowing recipients to verify that data comes from you and is valid.
    For example, a school could prove that test scores came from them
    and were not tampered with. (Institutions should use this more!)

The `--clearsign` option will wrap the message in an ASCII-armored
signature but will not otherwise modify its contents. This allows even
the losers who don't use gpg to read the body of the message, but allows
gpg users to verify that you wrote it and that the message wasn't
changed.

`gpg --clearsign filename`{.input}\
\

    -----BEGIN PGP SIGNED MESSAGE-----
    Hash: SHA256

    I vote YES on this important measure.

    -----BEGIN PGP SIGNATURE-----
    Version: GnuPG v1
    Comment: See Alan's GPG guide at https://futureboy.us/pgp.html

    iQIcBAEBCAAGBQJT3MFeAAoJEF8rR1bthz0jslMP/RMRODVKLmLwZ3sMR62COGc/
    0yQSh3c37qkkVjD0RvgdziHuCSSYelhNl7UMQofpdLonnJgPW3svlftE3Gn11JLp
    ZYv2iMwCzwyM2eLYpSQoJBNnGZzQDGnZRBkFOwdkkohUSBjhPjiszYw3KwnpsuxG
    I+m81IMJATR0wOylLumVdjbvS1/f9bOzBRvhgu2HS54lfPnl162RRZpycrrb5IOi
    07QWIlUGVUdAxFUq4Jlm99KB17lQhri3zm6m7O5k0faD3IKFRTQGKseq7j88pRs6
    j85v/cc35CHW9+66jcz7Y3UtOIj3gqDQd/Wj05YP01QSwSCuuVAezvXngljF8fLP
    OKQhFpLoLnWvDPgX3nKwGbX52qZwLGN0bZduhOmMPYwKAEFAYDOOW7q+i/dyz5xT
    od54j32QiNkSqDCVkvOT6dKiCdCa8GvtwwXPKa9X7+VZB2xYeJorJiaIesD7wyVN
    CQDx11uMGMkpZ/BmCIA5mDIkDnUTIxHxNFpn2kS6nHJqmJ/LleTpAKLhPWuY1U28
    YVraBzmAZ/Wj2Frq0utPi4cFf5r3x9jXIzie4fYrUjMKCN+CNfLL15Py/z9OY1ux
    vvYdMiLAzL1Ujvjpyw7sCdc2KnbXaM9jmbBGjmVCMX/wGcGKT6cIxYnkR4NOW62L
    jaBgelaHIL5kZ+E/kpS6
    =wh+e
    -----END PGP SIGNATURE-----

### Verifying Signatures

People who have verified your public key can verify messages that you've
signed by passing the output back into gpg:

`gpg --verify vote.txt.asc`{.input}\
\

`     gpg: Signature made Sat 02 Aug 2014 04:45:50 AM MDT using RSA key ID ED873D23 gpg: Good signature from "Alan Eliasen <eliasen@mindspring.com>"    `{.output}

If they haven't verified and signed your public key, then they will be
warned that the key is untrusted. This means that all that they can tell
for certain is that the message wasn't corrupted in transmission, *but
it really could have been written by anyone!* Beware "Untrusted good
signature!" It means that the signature is by someone whose fingerprint
you haven't verified.

### Detached Signature

Sometimes you want to sign a file, but without modifying it like the
`--clearsign` option above does, because people would need to edit the
file or use gpg to get at the contents.

Say, you're sending an executable file to someone. You don't want to
tamper with the executable file, but executable files are scary and
potentially very dangerous. So how can you guarantee to the recipient
that nobody has tampered with the file and that it actually came from
you? By creating a "detached signature" which is a separate file that
contains a signature for the specified file. This is achieved through
the `--detach-sign` command:

`gpg --detach-sign filename`{.input}

Then you ship the signature file along with the original file. The
recipient can verify that you signed the file and that it has not been
modified with the `--verify` command:

`gpg --verify filename.sig`{.input}\
\

`     gpg: Signature made Sat 02 Aug 2014 04:45:50 AM MDT using RSA key ID ED873D23     gpg: Good signature from "Alan Eliasen <eliasen@mindspring.com>"    `{.output}

### Proving You Wrote Something but Remaining Temporarily Anonymous

Let's say you found out that a huge company (we'll call them Mapple)
wrote a really crappy incompetent insecure website that leaked a lot of
their customers' information that anyone could access trivially by
adding 1 to a number.

Now, you're not sure if the company is awesome and honest and will pay
you a handsome bug bounty for pointing out their incompetent security
hole and helping them protect their customers' information, or if they
are psychotic morons who will claim *post-facto* that your access of
information they intentionally published on a public webserver without
any access control was "unauthorized" and have you charged under the
insanely incompetently-written and outdated Computer Fraud and Abuse Act
([CFAA](https://www.eff.org/issues/cfaa)).

So, how do you report this anonymously? Well, one very strong way would
be to generate a new keypair without your name on it, publish that
public key, and sign all your messages with the corresponding secret
key. This lets you do a few things:

-   You can prove that all subsequent messages signed with the same key
    are from the same person, even if you jump to different e-mail
    addresses or communication channels.
-   If they decide to be honest and offer you a bounty for your services
    to them and their customers, you can prove in the future that you're
    the person in possession of the corresponding secret key that signed
    the messages, for example, by decrypting something sent to you
    encrypted with your public key. Nobody else would be able to falsely
    claim that they're the submitter without verifying that they have
    the corresponding secret key.
-   If they are evil about it, you can remain anonymous to them. If you
    want to prove to others that you made the disclosure, you can, by
    signing a message with the same secret key or decrypting information
    sent to you that was encrypted with your public key (by using your
    secret key.)

(This is a mathematically super-strong version of the old trick of
ripping a dollar bill in half, and sending half of it to someone. If
they want to verify your identity, only you will have the other half of
the bill. A dollar bill, with distinctive tearing pattern and matching
serial numbers, is hard to forge.)

Updating Keys
-------------

People are constantly updating their keys for various reasons:

-   Keys get compromised or lost and they are revoked.
-   Keys are signed by more people, building a [Web of
    Trust](#WebOfTrust).
-   Users change the encryption algorithms they prefer. (See the [Using
    Stronger Algorithms](#StrongerAlgorithms) section for more about
    this.)

Updates to keys can be published to public key servers, including new
signatures. You can periodically update your keys by using

`gpg --refresh-keys`{.input}

This lets you ensure that the keys you're using haven't been revoked.
You might even find that more people have signed your public key. (And
they better have validated your key fingerprint and your identity using
the [verification procedure](#ProcedureForVerification) outlined above,
or they can't be trusted to sign keys properly and you should assign
them a low trust rating!)

Note that other people can sign *your* public key and upload the signed
key to a public webserver! So you might even find that your own key has
been updated!

### Updating Keys in Enigmail

Enigmail can update all of the keys in your keyring from a public key
server. The way to trigger this is from the menu items: `Enigmail` |
`Key Management` | `Keyserver` | `Refresh all Public Keys`. Again, I
might suggest that `pgp.mit.edu` has been a reliable keyserver for me.

### Listing Your Keys

You can get a list of the keys on your keyring and their corresponding
key IDs with:

`gpg --list-keys`{.input}

If you enter part of the name or e-mail address or key ID as the last
argument on the command-line, then only keys that match that pattern
will be listed.

`gpg --list-keys Alan`{.input}

### Who Signed My Key?

Now that you've updated keys from a keyserver, you might want to see who
has signed your key. After all, *anyone* can sign *any* key and
re-upload that key to a key server. You can see the signatures with the
`--list-sigs` command to gpg:

`gpg --list-sigs your@email.address`{.input}

In Enigmail, you can see the signatures for a key by going to
`Enigmail     | Key Management`, searching for a key, right-clicking on
that key, and then choosing `View Signatures`.

Or you can browse your key on a public keyserver, like
[pgp.mit.edu](http://pgp.mit.edu/). This is advantageous because if you
haven't imported someone's key yet, they will just show up as a key ID
number.

Again, if someone signed your key without validating the fingerprint
with you, they are actively damaging the web of trust. You should import
their public key just so you can tell your software to actively distrust
it as outlined in the [Signing a Key](#SigningAKey) section.

(After I published this document, an out-of-control signer whom I've
never met signed my key and published the changes to a public website. I
had to download his public key so I could tell gpg to actively distrust
his signatures!)

Building a Web of Trust
-----------------------

In the examples above, I stress the importance of *verifying* people's
public keys with them. But sometimes you can't do that directly. So how
can you verify someone else's public key?

Let's say I want to talk to Bob. I've downloaded a public key with his
name from a keyserver, but I can't be sure that key belongs to him. I
could maybe call him on the phone and verify his key that way, but I
don't know his voice, and I don't have his phone number. Or maybe he's
even under duress.

Luckily, my friend Alice has signed his public key. I trust Alice to
have verified his key properly. I have validated and trusted Alice's
public key personally. Thus I have a good reason to believe that Bob's
key really belongs to him.

This is why it's important to validate other people's keys very
carefully and to build a web of trust--so you can communicate with
people whose keys you can't personally verify.

See the [Signing a Key](#SigningAKey) section above to see how to sign
someone else's key and upload it to a keyserver.

Conversely, you may *not* want to publicly sign the keys of people you
communicate with. You may not want others to know who you communicate
with. You may have more than one keypair, and use them selectively for
communications with a single person once they've demonstrated strong
cryptographic practices.

This is serious business. [An example from
Syria](http://www.cjr.org/feature/the_spy_who_came_in_from_the_c.php?page=all)
shows how people die when others don't protect their communications.

If you don't want anyone to be able to analyze who you're talking to,
even by traffic analysis of key IDs, you can specify [hidden
recipients](#HiddenRecipients) in your messages.

Good Encryption Practices
-------------------------

By using encryption improperly, you can make your encrypted
communications easier to break. Some of the tips here are speculative
and may not apply to all cryptographic algorithms, but many
cryptographic algorithms are subject to common types of attacks. These
tips will help mitigate those potential weaknesses if algorithms are
found to be vulnerable to these types of attacks.

*TODO: Improve ALL THE THINGS.* [Send me more examples of good and bad
cryptographic practice, and ciphers that have been broken by poor
cryptographic practice.](mailto:eliasen@mindspring.com)

-   **Don't be predictable.** This is the way that much crypto has
    historically been broken--by knowing words or phrases that are
    likely to occur in the message. This is known as a
    ["known-plaintext"](https://en.wikipedia.org/wiki/Known-plaintext_attack)
    attack. For example, the WWII German Enigma machine codes were
    partially broken because people would end with expected phrases like
    "Heil Hitler!" or from spelling out numbers. (Looking for the number
    "eins", (1), the most common number, was a useful tactic in breaking
    Enigma.)
    You think this is academic and known-plaintext attacks can't happen?
    Well, take a look at [this recent break on the widely-used RC4
    cipher](http://sac2013.irmacs.sfu.ca/slides/s9.pdf). (It's used in
    SSL/TLS and in WEP/WPA in wi-fi.) It was found that if you knew a
    small amount of plaintext, you could recover the rest of the message
    (given a fairly large amount of encrypted communications, to be
    sure.) With as little as 6 bytes of plaintext, and a large number of
    communications, the rest of the message could be decrypted with high
    probability. (The more bytes are known, the easier it is to break.)
    Also, keep in mind that breaks in cryptographic algorithms only get
    worse.
-   **Don't be polite.** As a corollary of the above, don't start and
    end your message with predictable phrases or pleasantries.
-   **Don't send HTML-formatted encrypted emails.** There's a large
    amount of predictable boilerplate in HTML.
-   **No signatures!** As a corollary of the above, when sending
    encrypted messages, don't include your usual .sig file with your
    name, e-mail address, phone number, password, website, company
    policy, etc.
    This doesn't mean "no cryptographic signatures!" You still want
    cryptographically strong signatures like the kind you get with
    `--sign`. Smart e-mail add-ons like Thunderbird with Enigmail can
    suppress your signature when using encryption. Or you should encrypt
    just the meat of your email (and not the signature) if you *need*
    that silly signature.
-   **Don't quote previously-encrypted text.** When replying to an
    encrypted message, *don't quote the original text.* Again, having
    large stretches of expected text has been the downfall of many
    cryptographic algorithms.
-   **Don't encrypt the same message multiple times.** Some codes have
    weaknesses that if the same plaintext message is encoded several
    times (say, to several different people, or to the same person
    multiple times,) then more information can be derived about the
    contents or the key. If someone isn't able to read your encrypted
    message, don't send it again. After all, they're not following good
    cryptographic practice if they can't read it, and you should limit
    encrypted communications with them. Or, if you must send it again,
    alter it as much as possible before encrypting and sending it again.
    If encrypting the same message to multiple people, encrypt to all of
    them at once (assuming you want them to know who you're
    communicating with. They will at least see the key ID numbers.)
-   **Don't have encrypted and unencrypted versions of the same
    information.** As [noted above](#Shred), gpg does *not*
    automatically delete the plaintext version of a file when you
    encrypt it! Read that section on securely deleting files if
    possible.
-   **Garbage is good.** One of the hard problems in cryptography is
    identifying when a message has been successfully decrypted. How do
    you know? When it all comes out as mostly alphanumeric characters?
    When its word frequency looks like English? Make it hard for the bad
    guys. Jam in a bunch of random bytes into your message if you can.
    It'll make it harder to even detect the fact that the message was
    decrypted properly. Send your friends encrypted random bytes every
    day just for fun because screw the surveillance state we live in! If
    everyone did this, it would be utterly prohibitive to try and
    decrypt all of the random data flying around.
-   **If it's received encrypted, store it encrypted.** Some e-mailer
    plugins will offer to decrypt messages and store the decrypted
    versions in your mail folder. Don't do this. It allows someone to
    mount a chosen-plaintext attack on you just by sending you an
    encrypted message. Yes, it will make your messages impossible to
    search for content. But that's good.
-   **Don't encrypt stuff from untrusted sources.** There is a class of
    attacks called a
    ["chosen-plaintext"](https://en.wikipedia.org/wiki/Chosen-plaintext_attack)
    attack. Some encryption algorithms can be weakened or completely
    defeated if the attacker is allowed to choose the text that you are
    going to encrypt with your key. Always refuse to encrypt something
    specific that a third party asks you to encrypt, especially if it's
    lengthy.
-   **Hide your encryption entirely!** There's a branch of cryptography
    called "steganography" which hides secret communications in
    innocuous places that are very hard to detect. For example, by
    slightly modifying the least-significant-bits in the pixels of a
    JPEG image, you can hide encrypted messages in pictures of kittens!
    Or, you can hide them by adding slight, undetectable noise to audio
    files.

    It becomes *very* difficult and expensive to determine that a
    particular image even contains steganographic content. That's the
    best way to hide your information, especially as the NSA has decided
    that using cryptography to protect your privacy is probable cause
    that you're a terrorist, and they allow themselves to keep encrypted
    content "for as long as necessary" to break it.

    I have built some web-based [Steganographic
    Tools](https://futureboy.us/stegano/) that let you experiment with
    steganography from your browser! If you want to be more secure, of
    course, you'll run the steganography tools on your own machine. That
    page tells you more about the `steghide` program. (Hint: in Fedora
    it's `yum install steghide` )

Symmetric Encryption/Decryption
-------------------------------

Sometimes you don't want to use public key encryption. You can use
old-fashioned "symmetrical" encryption where everyone shares a common
password. In gpg, you do this by using `--symmetric` instead of
`--encrypt`:

`gpg --symmetric filename`

gpg will then prompt you for a password.

**Warning:** (I'm repeating this again.) When gpg encrypts or decrypts a
file, it usually *leaves the original file intact!*. You must remember
to delete the original file yourself, securely if possible. See the
[warning above](#Shred) for more details on how to do this.

If you want to paste the encrypted file into an e-mail or something, you
can use the `--armor` option.

The encrypted file can be decrypted by passing it back into gpg:

`gpg filename.gpg`

If you want to force the encryption algorithm used (the default is maybe
CAST5), you can add the `--cipher-algo name` command-line option, for
example `--cipher-algo AES256` . The list of available encryption
algorithms in your version of gpg can be found by running the
`gpg --version` command.

Symmetric encryption has its problems. It doesn't let you simultaneously
sign the message to indicate that it hasn't been tampered with or
replaced with another file that someone else generated! (You can,
however, sign it manually later using the techniques in the [Signing
Messages](#SigningMessages) section, but it's theoretically possible
that an attacker can replace that file in the brief time between when
you encrypted it and when you signed it.)

If you use symmetric encryption, you also need to solve the age-old
problem "how do I communicate the password securely?"

Why Public-Key Encryption is Cool
---------------------------------

-   In short, public-key encryption solves the age-old problem "how do I
    communicate a password securely?" You no longer have to. You just
    need the other person's public key, which can be published to the
    world.
-   You can also encrypt a message *that you can not decrypt!* This may
    sound silly, but you may want to write something to someone *that
    you cannot ever possibly be compelled to decrypt!* It will be
    impossible for you to decrypt, even though you wrote it and
    encrypted it and even if you have the file in your possession and
    even if you have all your secret keys and you know all of your own
    passwords and have them written down! That is cool. (You can smile
    serenely while they're beating you with a rubber hose, knowing that
    you can't endanger the lives of your sources, nor give up your
    rights, even if you felt like that might be entertaining for a
    change.) You can see how to do this physically in the [Encrypting
    Messages You Can't Decrypt](#OneWayEncryption) section.

    This actually has many important and practical uses:

    -   If you're a reporter (or other human) traveling abroad, you can
        encrypt materials using public-key encryption, to someone else's
        key, but *without* encrypting to your *own* public key.
        (**Warning**: some tools will encrypt to yourself by default.
        Read on.) It's easy to create a message that you can *never
        possibly* decrypt yourself, and cannot possibly be compelled to
        do so! Ever! You could encrypt them, say, using only the public
        key belonging to your newspaper's editor or lawyer. (And if your
        newspaper's editor and lawyer don't have public keys, have them
        [contact me](mailto:eliasen@mindspring.com) and I will help
        them. They need to do this. Now. Before they kill people.) You
        can be detained and couldn't ever be compelled to give up the
        password, as *you never had it!*

        You don't have to be in
        [Syria](http://www.cjr.org/feature/the_spy_who_came_in_from_the_c.php?page=all)
        (although journalists who don't use encryption kill people; read
        the link) or North Korea for this type of Orwellian police state
        coercion to happen. Even the otherwise-civilized United Kingdom
        has vile horrendous laws [that can jail you without trial if you
        don't give up passwords.](http://www.bbc.co.uk/news/uk-23776243)

        Edward Snowden has also stated that he has in his possession
        encrypted documents that he cannot possibly be compelled to
        decrypt, even under torture. (But maybe other trusted people
        potentially can decrypt them.) Public-key encryption is probably
        what he was hinting at. Nice work.

        Also see the [Hidden Recipients](#HiddenRecipients) section of
        this document to see how to hide the people to whom you've
        encrypted. That may be *very* important for journalists or
        dissidents or ordinary people who want to assert their rights to
        free association. It also allows you to post encrypted messages
        to public forums without anyone knowing who you're talking to.

        Also see my [Steganography tools](/stegano/) which let you hide
        the fact that any hidden communications are happening at all!
        You can hide secret communications in pictures of kitties.

    -   Let's say you have a web server that collects very sensitive
        user information. You don't trust the security of the web
        server, but you have to keep the information on that web server
        for a while before you move it elsewhere. Say, to a computer
        completely disconnected from the outside world. With public key
        encryption, you can encrypt information with a public key stored
        on the web server. However, the secret key would not ever be
        kept on that server! Even if someone breaks your web server wide
        open and has total access to *every single file*, *and* every
        single algorithm, *and* the public key, they will still *never,
        ever* be able to decrypt the private information on the server
        *because the secret key needed to decrypt it is not on the
        server at all!*
        [Miracles!](https://www.youtube.com/watch?v=N_2wK4LWvJA)
    -   If you rent space in a server farm, this can prevent malicious
        administrators at the hosting company (who probably hold
        superuser access on your machine, and can read all your files)
        from being able to do anything with your data. And it keeps your
        web server administrator or database administrator from seeing
        that sensitive data, *even if they have complete access to every
        file on the computer.*
    -   A real-world example of storing sensitive communications: The
        Federal Communication Commission's (FCC's)
        [Lifeline](http://shns.com/privacy-on-the-line) subsidized
        cell-phone program for low-income people leaked highly sensitive
        customer information for over 170,000 people, including Social
        Security numbers, birth dates, home addresses, and sensitive
        details about family finances from a public web server. Think
        about how you could use public-key encryption to collect and
        encrypt this data securely on the webserver, and only be able to
        decrypt it somewhere else much safer.

    Again, see how to do this in the [Encrypting Messages You Can't
    Decrypt](#OneWayEncryption) section.

-   It's easy to revoke access to one member of a group. If everyone in
    a group shared a password, it would be very difficult to remove one
    person's access. A different password might have to be created, and
    that password would have to be communicated securely to *all* other
    members of a group. Public-key encryption means that you can control
    exactly who is allowed to read future communications. If you don't
    want someone to read it, just stop encrypting to that person's
    public key. Even if they can still see your encrypted communications
    (like on a public mailing list,) they will no longer be able to
    decrypt it.

Fun Tips and Tricks
-------------------

Here are a collection of fun tips and tricks and puzzles for using GPG.
Please [send me more.](mailto:eliasen@mindspring.com)

### Using Stronger Algorithms

This section is optional but important.

By default, gpg uses weaker encryption algorithms than it could
(especially if you generated your keys using an older version of the
software.) This is to ensure compatibility with older versions.

Part of your public key specifies your preferences for the encryption
algorithms that you want people to use when communicating with you.
These are, by default, somewhat weak. You can view and modify these
preferences to make your communications stronger.

To view all of the algorithms supported by your version of gpg, type:

`gpg --version`

This will give an output that looks something like this:

`gpg (GnuPG) 1.4.14 Copyright (C) 2013 Free Software Foundation, Inc. License GPLv3+: GNU GPL version 3 or later <http://gnu.org/licenses/gpl.html> This is free software: you are free to change and redistribute it. There is NO WARRANTY, to the extent permitted by law.  Home: ~/.gnupg Supported algorithms: Pubkey: RSA, RSA-E, RSA-S, ELG-E, DSA Cipher: IDEA, 3DES, CAST5, BLOWFISH, AES, AES192, AES256, TWOFISH,         CAMELLIA128, CAMELLIA192, CAMELLIA256 Hash: MD5, SHA1, RIPEMD160, SHA256, SHA384, SHA512, SHA224 Compression: Uncompressed, ZIP, ZLIB, BZIP2`

You can modify your public key's cipher preferences by interactively
editing your key:

`gpg --interactive --edit-key your@email.address`

This will display a list of matching public keys. You may need to enter
the number of your key in that list so you can edit it.

*Hint:* You can always type `help` at the `gpg>` prompt to see all
available commands. There's lots of fun stuff hidden in here.

Next, show your current algorithm preferences by typing at the `gpg>`
prompt:

`showpref`

Which produces something like:

`Cipher: AES, TWOFISH, CAST5, BLOWFISH, 3DES      Digest: RIPEMD160, SHA1      Compression: ZLIB, ZIP, Uncompressed      Features: Keyserver no-modify    `

The protocols listed first will be used first. Note that the preferences
listed are probably not as strong as your copy of GPG supports, and
often the stronger algorithms are not requested at all! You can change
these preferences by calling the `setpref` command. I recommend
something like:

`setpref AES256 CAMELLIA256 AES192 CAMELLIA192 AES CAMELLIA128 TWOFISH CAST5 3DES SHA512 SHA384 SHA256 SHA224 SHA1 RIPEMD160 ZLIB BZIP2 ZIP Uncompressed`

You may want to add other algorithms that your software supports, or you
may want to disallow algorithms that you think are too weak.

You can see that it worked by typing:

`showpref`

Check this very carefully. If everything worked right, you can `save`,
(in some versions there's just `quit`) and you will be prompted if you
want to save your changes:

`save`

**Note:** You should then re-upload your key to a public key server and
send it to the people you communicate with. *Until people have imported
your new key, they will still be using the old algorithms when
encrypting to your public key!*

**Warning:** Note that the [OpenGPG Key
Management](http://www.gnupg.org/documentation/manuals/gnupg/OpenPGP-Key-Management.html)
document states:

> "When setting preferences, you should list the algorithms in the order
> which you'd like to see them used by someone else when encrypting a
> message to your key. If you don't include 3DES, it will be
> automatically added at the end. Note that there are many factors that
> go into choosing an algorithm (for example, your key may not be the
> only recipient), and so the remote OpenPGP application being used to
> send to you may or may not follow your exact chosen order for a given
> message. It will, however, only choose an algorithm that is present on
> the preference list of every recipient key."

This means that if you're encrypting to several people at the same time,
you can only use the strongest algorithm that the weakest person uses.

*Corollary:* Don't be the weakest link in your group! If you are still
using weak encryption preferences, you are bringing down the security of
the *entire group* you're communicating with. You are not weakening the
security of your own communications, but those of *everyone you
communicate with!*

*Corollary:* Inform the weakest links in your group that they could be
using stronger ciphers. Point them to this section [(Stronger
Algorithms)](#StrongerAlgorithms) of the documentation and help them fix
it. Get their updated public key and help them test their preferences
using `showpref` as described above.

*Corollary:* [Update your keys](#UpdatingKeys) often, so if someone on
your keyring chooses to use stronger algorithms, you respect their
preferences.

**Technical Note:** You may be wondering how these encryption algorithms
like AES are even relevant to you if you chose to, say, generate an RSA
or DSA public key. *RSA and DSA are public-key encryption algorithms,
after all, and AES is a symmetric encryption algorithm! I thought we
were using public-key encryption here!* The answer is that decrypting an
encrypted communication in GPG is done in two stages, with both
public-key and symmetric algorithms being used:

1.  **Public-key decryption**: GPG uses your secret encryption key to
    decrypt a session-only secret key that was encrypted with your
    public (RSA or DSA) key.
2.  **Symmetric decryption**: GPG uses this session-only secret key to
    decrypt the "body" of the message which was encrypted using a
    symmetric algorithm like AES.

Your public key (RSA or DSA) is only used for the first step. The actual
body of the message is encrypted with a (faster) symmetric encryption
algorithm, so it's important to make sure that you're using strong
algorithms for both phases.

### Verbose Information

You can use the `-vv` command-line option to gpg to give verbose output
about what algorithms are actually being used. (Note that if you're
pasting in decrypted text, after you're done pasting, you may need to
send your operating system's "end-of-file" character. This is `Ctrl-D`
in most Unixlike systems and `Ctrl-Z` in Windows-like systems.)

`gpg --list-packets` can list the packets of any GPG file and give
details on what's contained therein. This tends to output
not-very-meaningful numeric data about which encryption algorithms were
used, but you can decode these by looking at the specification for the
Open PGP standard, [RFC 4880](https://tools.ietf.org/html/rfc4880),
specifically [Section 9](https://tools.ietf.org/html/rfc4880#section-9).

You can also use programs like [pgpdump](http://www.pgpdump.net/) to see
what's included in a PGP message.

Also see the [Automating GPG](#Automating) section below to see more
options for dumping detailed information about what GPG is doing.

### Requiring Multiple Decrypts

You can encrypt documents that require several people must cooperate to
decrypt, by encrypting with multiple passes, specifying a different
recipient each time. They will need to decrypt in the reverse order that
you encrypted.

*TODO: Make an example, preferably one that writes no intermediate files
(e.g. output to stdout using `--output -`) and doesn't make you enter
passwords multiple times. Naïve versions make gpg complain with weird
"broken pipe" errors and races in password entry.*

### Hidden Recipients

Sometimes you want to hide the recipients of your message from any
snoopers. Normally, the key IDs of the recipients are part of the
message. However, you can hide these by specifying
`--hidden-recipient recipient` for each recipient you wish to remain
hidden (instead of using the `-r` or `--recipient` flag to specify
recipients.) The decrypting program will have to try all available
secret keys to try and decrypt the message. (Hidden recipients' key IDs
show up as all zeroes in the encrypted message.)

The `--throw-keyids` command-line option is essentially the same as
using `--hidden-recipient` for all recipients.

There are other interesting options for hiding recipients in the [GPG
key-related
options](http://www.gnupg.org/documentation/manuals/gnupg-devel/GPG-Key-related-Options.html)
documentation.

### Encrypting Messages You Can't Decrypt

The section [Why Public-Key Encryption is Cool](#Cool) explains reasons
that you might want to create an encrypted message that you can never be
compelled to decrypt. This section discusses how that is performed.

#### In GPG

When you encrypt a message in GPG from the command-line, it does *not*
encrypt to you by default! You would need to specify your *own* e-mail
address as a recipient with the `-r     recipient@email.com` option for
you to be able to decrypt it.

(See the [Manually Encrypting for E-mail](#ManuallyEncrypting) section,
including the warning, or the [Encrypting Files](#EncryptingFiles)
section, including the warning.)

Thus, there's nothing to do when using gpg on the command-line other
than remembering *not* to specify your own e-mail address as a
recipient. (Note: You can change the "encrypt to self" behavior in your
`gnupg.conf` file, so be careful if you've modified that.)

This is why I encourage people to learn and use the GPG command-line for
sensitive communications. Its defaults are usually safer than what your
e-mail program exposes to you. See below for Enigmail (and its
problems.)

#### In Enigmail

**Global solution:** You can turn off encrypting to yourself by default
from the main Thunderbird menu: `Enigmail | Preferences |    Sending`
and uncheck `Add my own key to the recipients    list`. **Warning:**
This means that you won't be able to decrypt any e-mails you send to
*anyone* after this, until you re-enable this setting! This is a global,
persistent setting, not a per-message setting!

**Per-message solution:** Enigmail currently doesn't seem to support a
good per-message solution. The only way to turn off signing to yourself
on specific messages requires two steps:

1.  Turn off signing to yourself using the "Global Solution" above.
2.  Make Enigmail prompt you for recipients to encrypt to every time you
    send a message. To enable this, from the main Thunderbird window,
    select: `Enigmail | Preferences | Key      Selection | Manually`.

Then, every time you send an encrypted e-mail, it will pop up a dialog
which allows you to select which identities on your keyring that you are
going to encrypt to. If you *do* want to encrypt to yourself (so you can
decrypt and read that message later,) you'll have to manually select
your own identity in the list. This is annoying. Note that if you don't
perform step 1.) above, *Enigmail will still encrypt to you even if your
name is unchecked in the list!*. Seems like a bug.

### Migrating to a New Key

This section of the document describes the process for migrating to a
new GPG key, which is two different but related problems:

-   Creating a new public/secret keypair key for yourself which you will
    then communicate to others.
-   Updating when someone else generates a new public key.

These are addressed in the sections below.

#### Creating Your Own New Key

Sometimes you want to generate a new public key for yourself, and
migrate away from the old one. There are a few steps to this process:

-   **Generate the new key.** For this step, you will probably want the
    old and new keys to co-exist on your keyring at the same time. As
    noted in the [Getting Started](#GettingStarted) section, you will
    begin the process of creating a new key with:

    `gpg --gen-key`

-   **Know your old and new key IDs.** Throughout most of this document,
    you use e-mail addresses to identify keys. However, once you have
    more than one key for a given e-mail address, things get a bit
    trickier. GPG behaves somewhat dangerously and uses the *first*
    secret key in your keyring, unless you explicitly tell it otherwise.
    Thus, you will need to know the key IDs of your old and new keys,
    and use them in the right places below.

    You can list your secret keys with:

    `gpg --list-secret-keys`

    or the equivalent:

    `gpg -K`

    (note that that's a capital `K`. A lowercase `k` lists all keys.)

    This produces output something like:

    ` sec   1024D/B05676B1 2002-06-26 uid                  Alan Eliasen (http://futureboy.homeip.net/) <eliasen@mindspring.com> ssb   1024g/70AC29FB 2002-06-26  sec   4096R/ED873D23 2014-07-22 uid                  Alan Eliasen <eliasen@mindspring.com> ssb   4096R/5314E70B 2014-07-22      `

    I have highlighted the key IDs in bold. They appear on a line
    beginning with `sec`. As you can see by the creation dates, the old
    key ID is `B05676B1` and the new key ID is `ED873D23`. Yours will be
    different, of course. Make a note of them.

-   **Create a revocation certificate for the new key.** This will let
    you revoke the key if you lose it. See the directions in the
    [Generating a Revocation Key](#RevocationKey) section of the
    documentation, but substitute your *new* key ID for the e-mail
    address. You may also want to change the filename if you already
    have a revocation key for your old key.
-   **Ensure that the new key uses strong cryptography preferences.** By
    default, the encryption preferences specified in your public key are
    probably not as strong as they should be. Follow the procedure in
    the [Using Stronger Algorithms](#StrongerAlgorithms) section of the
    documentation, but substitute your new key ID for your e-mail
    address. That is, the command-line will be:

    `gpg --interactive --edit-key newKeyID`

-   **Sign the new key with your old key.** If people have your old key,
    this helps them trust that the new key was generated by you.

    When signing a message, the gpg options `--local-user       keyID`
    or the equivalent `-u keyID` lets you specify which key is doing the
    signing. Thus, to sign the new key with your old key, you would use
    the command:

    `gpg -u oldKeyID --sign-key newKeyID`

-   **(Optional) Trust the old key's signatures.** You may have signed
    other peoples' keys with your old key. You can tell the new key to
    trust signatures made by the old key using the procedures in the
    [Signing a Key](#SigningAKey) section, specifically the `trust`
    command. The command-line may look like:

    `gpg -u newKeyID --interactive --edit-key oldKeyID`

    And then using the command `trust` followed by `save`. (Which in
    some versions is just `quit`.)

-   **Set the new key as your default key.** As noted before, GPG uses
    the *first* secret key in your keyring to sign messages. You thus
    have a few options to make gpg use your new key by default. Choose
    one of the options below:
    1.  **(Recommended)** Set the `default-key` option in your
        `gpg.conf` file to your new key ID. (See the [Sandbox](#Sandbox)
        section to see where your `gpg.conf` file may reside.) The line
        in the file will look something like:

        `default-key newKeyID`

        **ENIGMAIL WARNING:** Even if you have set this default key, and
        disabled your old key, *Enigmail will still use the old,
        disabled key to sign your messages! It ignores gpg's
        `default-key` setting and does something very dangerous and
        wrong to choose the signer! In fact, Enigmail probably ignores
        **all** your settings in your `gpg.conf` file and does its own
        broken, random thing.*

        To work around this, you apparently need to tell Enigmail what
        your new key is explicitly. This setting is hard to find. The
        place to configure this is currently hidden under each e-mail
        account on the (usually) left-hand side of your screen under
        `OpenPGP        Security` where the option
        `Use specific OpenPGP key        ID` should be checked, and your
        new key ID entered in the box.

        Here's the [current screenshot from the Enigmail
        project](https://www.enigmail.net/documentation/per-account.php)
        showing where this setting should be configured for each
        account.

        [This e-mail
        thread](https://www.enigmail.net/list_archive/2008-June/009469.html)
        from an Enigmail/Mozilla engineer corroborates some of this
        scary, dangerous awfulness.

    2.  **(Not recommended)** This is ponderous and easy to forget, but
        you can specify the new key ID on the command-line with each
        signing command: `-u newKeyID`
    3.  **(Optional)** Disable the old key in your keyring. You'd think
        that this should not be necessary if you followed step 1, *but
        be warned that GPG and Enigmail will encrypt to the old key ID
        and sign with the old key ID if you specify your e-mail address
        as one of the recipients, as it uses the first key that matches
        the e-mail address.* Ugh. The command would be:

        `gpg --interactive --edit-key oldKeyID`

        And then using the command `disable` followed by `save`. (Which
        in some versions is apparently just `quit`). You can
        theoretically re-enable it in the future using `enable`.

    4.  **(Optional, possibly dangerous)** If you're *absolutely sure*
        that you'll never need the old secret key, you can delete it.
        Keep in mind that this will make it impossible for you to
        decrypt any old communications that were encrypted to the old
        key! You probably don't want to do this, so I'm not going to
        tell you how, (but I'll say that the `help` command from the
        `--edit-key` mode is your friend, and contains lots of
        interesting tricks. Take a look!)

        Because of the glaring problems and outright bugs in Enigmail
        and GPG's handling of multiple keys for the same e-mail address,
        it's not a bad idea to delete the old key when you can finally
        be free of it.

-   **Communicate the new key to people who have your old key.** One of
    the best ways to do so is to create a migration document that
    explains your reasons, your old and new key information, and sign
    that message with your *old* key using:

    `gpg -u oldKeyID --clearsign [filename]`

    I have a [sample migration document](gpgmigration.txt) that you are
    free to use and modify.

-   **Import the new signatures from your friends.** People may publicly
    sign your key and return it to you, or upload the signed key to a
    keyserver. See the [Signing a Key](#SigningAKey) section of the
    documentation for more information. Also, be sure to periodically
    refresh your keys from a public keyserver using:

    `gpg --refresh-keys`

-   **(Optional) Upload the new key to a keyserver.** See the
    [Publishing your Public Key](#Publishing) section for how to do
    this. This step is important if people have signed your key and sent
    it back directly to you, as their signatures will not appear on
    public keyservers until *someone* uploads to a keyserver.
-   **(Optional, Potentially Dangerous) Revoke the old key.** If you
    know what you're doing, you can (and eventually should) revoke the
    old key. Since this is somewhat dangerous, I'm not going to give you
    explicit steps, but [this section of the GPG
    guide](https://www.gnupg.org/gph/en/manual/c14.html#REVOCATION) will
    get you started. (Link opens in new window.)

    Revoking a public key is not the end of the world, though. That
    guide notes that:

    > "A revoked public key can still be used to verify signatures made
    > by you in the past, but it cannot be used to encrypt future
    > messages to you. It also does not affect your ability to decrypt
    > messages sent to you in the past if you still do have access to
    > the private key."

    However, this paragraph is deceptive if not outright wrong! People
    *can and will* continue to encrypt future messages to you using the
    revoked key *if they don't know about the revocation, and haven't
    updated your key!* They will only know about the revocation if they
    periodically refresh your key from a keyserver using something like:

    `gpg --refresh-keys`

    Since you have no guarantee that people do that (and few people do
    it regularly, in my experience,) then you need to make sure that you
    communicate the revocation to people you have communicated with in
    the past. Again, see the "Communicate the new key..." section above
    for a sample document explaining how to do this.

#### Using Someone Else's New Public Key

People that you communicate with may generate new public keys, and you
need to ensure that the new key is valid, and that you are using the new
key instead of the old key. There are a few steps to this process:

-   **Import the new key.** If the person emails you the new key
    directly, it should be trivial to import. Otherwise, you can import
    it with

    `gpg --import`{.input}

    either specifying a filename to read from or pasting the new key in
    directly. (When you're done pasting, you may need to send your
    operating system's "end-of-file" character. This is `Ctrl-D` in most
    Unixlike systems and `Ctrl-Z` in Windows-like systems.)

    You may also fetch the new key from a keyserver. Be sure to read on
    and validate that the person actually uploaded it!

-   **Know their old and new key IDs.** Once you have multiple keys for
    a person, GPG behaves very badly. *It uses the key for the **first**
    e-mail address that matches, and ignores the others!*

    For the next few steps, you will need to know the key IDs for the
    old and the new keys. You can list all keys associated with their
    e-mail address by doing:

    `gpg --list-keys their@email.address`

    or the equivalent:

    `gpg -k their@email.address`

    This produces output something like:

    ` pub   1024D/B05676B1 2002-06-26 uid                  Alan Eliasen (http://futureboy.homeip.net/) <eliasen@mindspring.com> sub   1024g/70AC29FB 2002-06-26  pub   4096R/ED873D23 2014-07-22 uid                  Alan Eliasen <eliasen@mindspring.com> sub   4096R/5314E70B 2014-07-22      `

    I have highlighted the key IDs in bold. They appear on a line
    beginning with `pub`. As you can see by the creation dates, the old
    key ID is `B05676B1` and the new key ID is `ED873D23`. Yours will be
    different, of course. Make a note of them. You will need them in the
    following steps.

-   **Validate the new key with the person.** You should always be
    warned that *anyone* can generate a public key for *any* e-mail
    address. *Anyone* can post that key to *any* key server, so you need
    to follow the instructions in the [Procedure or
    Verification](#ProcedureForVerification) section of the document to
    validate that key with the person!

    If the person has signed the new key with the old key, (and they
    should have!) then you can perform another procedure to have a
    strong certainty that whoever is in control of the old key created
    the new key. (But if the old key was stolen/compromised, you need to
    be extra careful!) You can check signatures on the new key by
    running:

    `gpg --check-sigs newKeyID`

    This will produce output that looks something like:

    ` pub   4096R/ED873D23 2014-07-22 uid                  Alan Eliasen <eliasen@mindspring.com> sig!3        ED873D23 2014-07-22  Alan Eliasen <eliasen@mindspring.com> sig!         B05676B1 2014-07-22  Alan Eliasen (http://futureboy.homeip.net/) <eliasen@mindspring.com> sub   4096R/5314E70B 2014-07-22 sig!         ED873D23 2014-07-22  Alan Eliasen <eliasen@mindspring.com>      `

    The exclamation points following `sig` are the important things
    here. The line in bold, with the old key ID, indicates that the old
    key (which you can identify by the key id you found in an earlier
    step) signed the new key and the exclamation point after `sig`
    indicates that the signature check passed.

    In Enigmail, you can get to this from
    `Enigmail     | Key Management`, searching for a key, right-clicking
    on that key, and then choosing `View Signatures`. You are looking
    for "Yes" in the "Valid" column.

-   **Sign the new key.** Once you have validated the new key with the
    person, you can sign the key. See the See the [Signing a
    Key](#SigningAKey) section above to see how to sign someone else's
    key, but note that you'll have to substitute the new key ID instead
    of the e-mail address, or GPG will likely just give you the first
    matching e-mail address (which is the old key):

    `gpg --interactive --edit-key newKeyID`

-   **(Optional) Send the signed key to its owner.** Again, see the
    [Signing a Key](#SigningAKey) section above to see how to sign
    someone else's key and export it for e-mailing, or to send it to a
    keyserver.
-   **Delete or disable the old key.** Since you now have both keys on
    your keyring and you no longer want to accidentally use the old key,
    you should delete or disable the old key.

    With all the problems with GPG and Enigmail's handling of multiple
    keys for the same e-mail address, deleting it is by far the safest
    option, but simply disabling it means that it *should* no longer be
    used for encryption (although the bugs listed above for Enigmail
    leave me with little confidence in its ability to choose the right
    key.) However, GPG may still trust signatures made by a disabled
    key, so if the other person's old key was stolen (and not revoked)
    then you might be at risk of accidentally trusting it!

    To disable or delete the old key, do:

    `gpg --interactive --edit-key oldKeyID`

    Check that you have the correct key, and then type either `disable`
    or `delete`. After that, type `save` and save your changes.

    Note that some versions of GPG appear not to have a `delete` command
    from the interactive menu, so you may have to do something like:

    `gpg --delete-keys oldKeyID`

    **From Enigmail:** From within Enigmail, you can disable or delete a
    key by the following: `Enigmail | Key Management`. Search for the
    key you want to modify, right-click it, and you have the option to
    delete or disable it.

### Keysigning Party

A keysigning party is just a bunch of repetitions of the [Procedure for
Verification](#ProcedureForVerification) described above. You meet other
people, validate their identities, and exchange fingerprints of your
public keys. Later, usually after the party, you can download their
public keys from a keyserver, verify that the fingerprint you got from
the person matches the one you downloaded from the keyserver, and then
sign the key and send the signed key to its owner. You don't need to
(and are often warned not to) bring a computer to the keysigning party,
as long as you are prepared using the guidelines below:

-   **Before the keysigning party:**
    1.  Print out a bunch of copies of your public key's
        [fingerprint](#Fingerprint) on strips of paper. Keep them safely
        in your possession until the keysigning party:

        `gpg --fingerprint your@email.address`

        It may look something like this (I've put the fingerprint, name,
        and e-mail address in bold.)

        `         pub   4096R/ED873D23 2014-07-22         Key fingerprint = EC23 92F2 EDE7 4488 680D  A3CF 5F2B 4756 ED87 3D23         uid                  Alan Eliasen <eliasen@mindspring.com>         sub   4096R/5314E70B 2014-07-22        `

        Here's a fancier one I printed out 4 to a page for a keysigning
        party at DEFCON: [DEFCON fingerprint
        document](fingerprint.html).

    2.  Bring a pen, some paper, and a photo ID. You may wish to obscure
        sensitive details on your photo ID (e.g. license number,
        address, birthdate) if you're not meeting with people you know
        and trust. Blue painter's tape works well for this.
    3.  If your key *is* on a public keyserver, then there is no step 3!
        You're ready! If your public key *isn't* listed on a keyserver,
        then either [publish it to one](#Publishing) or, (less
        friendly,) provide a way for others to download it. (Say, by
        publishing a URL on the paper that contains your fingerprint.) I
        definitely *don't* recommend exchanging flash drives at a
        keysigning party!

-   **During the keysigning party:**

    For each person you meet at the keysigning party:

    -   Exchange paper copies of your fingerprints. You should both give
        and receive one, but it does not necessarily have to be
        symmetrical. (If you run out of pieces of paper, you can always
        copy fingerprints by hand, or take a picture of one, etc.)
    -   Attempt to validate the other person's identity, usually by
        asking to see their photo id if you don't know them otherwise.
        Be courteous. You don't have to share your ID with anyone you
        don't want to, and they don't have to share with you. Again,
        it's good to mask out sensitive details on your ID, (like with
        blue painter's tape.)
    -   Once the identity is validated, sign or initial the fingerprint
        you received from them, and keep it in a secure place. You will
        need it later.
    -   (Optional) Go around the room in a group with people you know.
        If you personally know someone that you're exchanging keys with,
        let your friends know that, and ask them to do the same.
        Introduce each other. It enhances the trust level.
    -   (Optional) Ask the person if they have a photo of themself in
        their public key. (You can attach a small photo to your public
        key, which makes it harder to impersonate you in person.) If
        they do, you might ask to take a picture of them to compare with
        the picture in the public key later.
-   **After the keysigning party:**

    *After* the keysigning party is when you usually do the actual
    signing of keys. For each person that you met:

    1.  **Import their public key from a keyserver.** Again, note that
        the last 8 or 16 hexadecimal digits of the fingerprint are their
        short or long public key ID, respectively. For example, if all
        you have is the fingerprint:

        `EC23 92F2 EDE7 4488 680D  A3CF 5F2B 4756 ED87 3D23`

        Then you can instantly determine the short key ID, which is the
        last 8 hexadecimal digits of that fingerprint (removing spaces),
        which gives `ED873D23`. (The long key ID is the last 16 digits.)

        With just that number, you can request their public key from a
        keyserver:

        `gpg --recv-keys keyID`

        You will see something like:

        `         gpg: requesting key ED873D23 from hkp server keys.gnupg.net         gpg: key ED873D23: public key "Alan Eliasen <eliasen@mindspring.com>" imported         gpg: 3 marginal(s) needed, 1 complete(s) needed, PGP trust model         gpg: depth: 0  valid:   2  signed:   0  trust: 0-, 0q, 0n, 0m, 0f, 2u         gpg: Total number processed: 1         gpg:               imported: 1  (RSA: 1)        `

        (You can even fetch public keys from keyservers using all 40
        digits of the full fingerprint (with spaces removed) but people
        usually use the short key ID because it's easier to type from a
        piece of paper. You will still verify the *full* fingerprint in
        the next steps.)

        You can also search for keys by e-mail address instead of key
        ID, using `gpg --search-keys their@email.address` but if you
        don't even have the e-mail address, the fingerprint alone is
        sufficient.

        (Note that with just an 8-hex-digit short key ID, it's possible
        that there may be key collisions when downloading from a
        keyserver. You can reduce this possibility by using the 16- or
        40-bit fingerprint. See the [Short key IDs are Bad
        News](#ShortKeyID) section of this document if you want to know
        more about key collisions.)

    2.  **Generate the local fingerprint of the key you imported**. This
        verifies that the public key you received has the proper
        fingerprint:

        `gpg --fingerprint keyID`

        Again, you could also search by e-mail address instead of key
        ID. See the [Fingerprint](#Fingerprint) section of this document
        to see how to verify fingerprints in Enigmail.

    3.  **Verify that this fingerprint matches the one you have on
        paper.** You just do this with your eyes, comparing the
        40-hexadecimal-digit numbers.
    4.  **Sign the key** if everything matches. See the [Signing a
        Key](#SigningAKey) section for detailed information on how to do
        this. You may sign the key publicly or locally. Signing the key
        tells your cryptographic software that you've validated the
        other person's identity and that your software no longer has to
        warn you that the key has not been properly verified and
        trusted.

        Since you have the key ID, the best way to generate the
        fingerprint, sign, and trust the key is to edit it interactively
        using a command like:

        `gpg --interactive --edit-key keyID`

        and then using the commands `sign` (which will show you the
        fingerprint, you can also generate it with `fpr`) and `trust`
        followed by `save` or `quit`. *Hint:* Type `help` for the
        interactive commands.

    5.  **If you've publicly signed the key, return the signed key to
        its owner.** This allows them to import your signature and share
        that signature with others. Again, see the [Signing a
        Key](#SigningAKey) section of this document for ways to do this.

        In some circles, it may be considered more courteous to email
        the signed key back to its owner rather than to upload the
        signed key back to a keyserver directly, but be warned that
        *anyone* can sign *any* key and upload it to any keyserver, so
        someone may do this without your knowledge or consent. In short,
        exporting the key for e-mailing back to its owner will probably
        look something like:

        `         gpg --armor --export keyID        `

        and then emailing that output to the owner of the key.

        On the other hand, you may not want to send an unnecessary
        encrypted message, so you can upload the signed key directly to
        a keyserver using:

        `         gpg --send-keys keyID        `

        Again, be warned that the key's owner and other people will not
        see or know about that signature until they do:

        `gpg --refresh-keys`

-   **When you receive your own signed key from others, import it.** See
    the detailed steps in the [Importing a Key](#ImportingAKey) section
    of the documentation above.
-   **Periodically publish your newly-signed key to a keyserver.** As
    you get new signatures, publish them to a keyserver. See the
    detailed steps in the [Publishing your Public Key](#Publishing)
    section of the documentation above. Most people won't see the new
    signatures until they're published to a keyserver!
-   **Periodically refresh keys from a keyserver.** See the detailed
    steps in the [Updating Keys](#UpdatingKeys) section of the
    documentation above to collect all the new signatures from the
    keysigning party. You may find that other people have signed your
    key and uploaded them directly to the keyserver. This also helps you
    collect the web of signatures from all the people who were at the
    keysiging party.

    In a nutshell, you can do this with:

    `gpg --refresh-keys`

-   **For fun, look at all your new signatures!** You can list the
    signatures using:

    `gpg --list-sigs your@email.address`{.input}

    If you see signatures that have `[User ID not found]` you might have
    better luck examining your key at [pgp.mit.edu](http://pgp.mit.edu/)
    or [sks-keyservers.net](https://sks-keyservers.net/).

Technical Notes
---------------

The rest of this document contains advanced technical notes. Please
[send me more.](mailto:eliasen@mindspring.com)

### Short Key IDs Are Bad News

As mentioned above, key IDs are usually specified as 8-character
hexadecimal strings. The GPG program makes it sort of hard to see that
your full key ID is actually a 16-character hexadecimal string. With
only 8^16^ (which is a bit over 4 billion) unique short key IDs, there
is a probability that there are collisions of short key IDs in public
key servers. That probability is 1, as we know collisions occur. (The
probability is infinitesimally close to 1 in mathematical analysis.)

With (at the time of this writing) over 3 million keys in public
keyservers, (obtained from [the sks-keyservers status
pages](https://sks-keyservers.net/status/)) there are likely many
collisions. One would first expect to see a collision with only about
82,000 keys in the keyserver.

The mathematics of finding the probability of collisions can be found in
the Wikipedia [Birthday
Attack](https://en.wikipedia.org/wiki/Birthday_attack) article.

There's more information in the interesting article [Short Key IDs are
bad news (with OpenPGP and GNU Privacy
Guard)](http://www.asheesh.org/note/debian/short-key-ids-are-bad-news.html)
which demonstrates real instances of key ID collisions.

*Summary:* it's safer to publish your 16-hex-digit key ID than your
8-hex-digit one. Read on to find out how to find that ID.

### Finding Your Longer Key ID

By default, GPG only shows 8-hex-character key IDs when you do something
like:

`gpg --list-keys eliasen@mindspring.com`{.input}\
\

` pub   4096R/ED873D23 2014-07-22 uid                  Alan Eliasen <eliasen@mindspring.com< sub   4096R/5314E70B 2014-07-22    `{.output}

You can change this to get long or short keys using the
`--keyid-format     short|0xshort|long|0xlong` option.

`     gpg --keyid-format long --list-keys eliasen@mindspring.com    `{.input}
\
\

` pub   4096R/5F2B4756ED873D23 2014-07-22 uid                          Alan Eliasen >eliasen@mindspring.com> sub   4096R/11C2E18C5314E70B 2014-07-22    `{.output}

You can get your also 16-hex-character key ID in a more
computer-parseable one-line format using the `--with-colon` option:

`     gpg --fingerprint --with-colon your@email.com    `{.input} \
\

` pub:u:4096:1:5F2B4756ED873D23:2014-07-22:::u:Alan Eliasen <eliasen@mindspring.com>::scESC: fpr:::::::::EC2392F2EDE74488680DA3CF5F2B4756ED873D23: sub:u:4096:1:11C2E18C5314E70B:2014-07-22::::::e:    `{.output}

The public key is the line that begins with `pub`. You can automate the
extraction with (on a Linux-like system):

`gpg --fingerprint --with-colon email@address.com    | grep '^pub' | cut -d: -f5,10`{.input}\
\
 `5F2B4756ED873D23:Alan Eliasen <eliasen@mindspring.com>`{.output}

However, read on to see a more common way to find the 16-hex-character
key ID using only the fingerprint.

### Key IDs and Hash Algorithms

You might not have noticed that your key ID is the final digits of the
[fingerprint](#Fingerprint) of your key. It took me a long time to
realize that.

A fingerprint is usually the SHA-1 hash of a key, which is 160 bits, or
20 bytes, or 40 hexadecimal characters.

Your short key ID is the last 8 hexadecimal digits of your fingerprint.
Your long key ID is the last 16 hexadecimal digits of your fingerprint.
So you can always find the long or short key ID if you have someone's
full fingerprint, and use that long or short ID (or the full
fingerprint!) to import from a keyserver.

### Enigmail, gpg-agent, and Gnome keyring bugs

This section describes workarounds for Fedora Linux (and perhaps other
Gnome and Mate environments) where Enigmail apparently remembers
passwords forever, even if you don't want it to.

I noticed that Enigmail never expired my gpg passphrase, even when I
told it to expire after 2 minutes of idle time. Even worse, it would
then *automatically and silently* decrypt PGP/MIME messages when I tried
to view them, even though I told Enigmail to *not* automatically
decrypt. That's dangerous. If an attacker adds lot of attachments, they
can mount known-cryptext attacks and recover your entire signing key,
even with an [acoustic attack](http://www.tau.ac.il/~tromer/acoustic/)
that never touches your computer!

Update: This is apparently a known bug, [Enigmail Bug
\#287](https://sourceforge.net/p/enigmail/bugs/287/).

I thought this was related to `gpg-agent`, which sometimes handles
passphrase input, so I tried putting the following into a new
`~/.gnupg/gpg-agent.conf` file to tell it to forget passwords after 60
seconds:

`default-cache-ttl 60`

However, that didn't work. I tried switching off "use gpg-agent for
passphrases" in the Enigmail advanced preferences, but that didn't work
either.

After further research, I found out that the Gnome and/or Mate desktop
environments were setting up their *own* GPG keyring daemons which just
weren't behaving well. (These processes may be called
`gnome-keyring-daemon` and/or `mate-keyring-daemon`. Note that this same
process name may be controlling your ssh keys as well, so you may not
want to kill them outright. Read on.) These can be turned off in
Fedora's main menu by going to
`System | Preferences | Startup    Applications| Startup Programs` and
unchecking `GPG Password    Agent: Gnome Keyring: GPG Agent` and since
I'm running Mate, also unchecking
`GPG Password Agent: Mate Keyring: GPG Agent`. (There are probably lots
of other things you might want to turn off in there.)

Enigmail then wouldn't talk to `gpg-agent` usefully so I cut it out of
the loop also. I disabled "use gpg-agent for passphrases" in the
Enigmail advanced preferences. After that, Enigmail popped up its own
gpg key dialog, and everything worked just fine, with Enigmail
forgetting the passphrase after the specified time.

Note that this may not work just fine if you're using `gpg2`, which may
require the use of gpg-agent, so you may have to work harder to set that
agent up correctly.

Please let me know if you have better workarounds.

### Automating GPG

If you're automating things, you can specify the password for encryption
and decryption with the `--passphrase password` command-line option.
Note that the password may get stored in your command history, will be
visible in a process list, etc., so this is generally a Bad Idea. You
can mitigate this somewhat with the `--passphrase-file filename` option.
Just protect that file! **Note:** In gpg2 and possibly some versions of
gpg, you will have to specify the `--batch` option for gpg2 to actually
use those passwords or passphrases! It doesn't hurt to specify it in
these cases. The `--batch` option also prevents gpg from popping up a
password entry field or anything requiring human interaction.

Signing a key with `--sign-key` still prompts you if you really want to
sign, even with `--batch` and a passphrase, but you can add the `--yes`
option to automatically choose "yes" to the prompts.

The gpg program usually sends a lot of status information to standard
error (stderr) but you might want that output directed elsewhere, or
sent to a file. The `--logger-file filename` or
`--logger-fd filedescriptor` will redirect that output.

For more machine-parseable output, there's a status file that can be
written using the `--status-file filename` or
`--status-fd filedescriptor` options. This gives lines that indicate
details of what was found in the message, what was tried, and the
detailed status of each step. More details about this output can be
found in the [Unattended
Usage](http://www.gnupg.org/documentation/manuals/gnupg-devel/Unattended-Usage.html#Unattended-Usage)
section of the GPG documentation.

For more fun, here are some [Esoteric GPG
Options](http://www.gnupg.org/documentation/manuals/gnupg/GPG-Esoteric-Options.html)
that you may need to know to automate GPG.

Read on to the next section to see how to specify where gpg stores its
configuration files and keys.

### Making a Sandbox / Multiple keyrings

Often, you'll want to experiment with GPG without actually making
changes to your primary keyring. You can easily create a "sandbox" to
make changes to a completely separate keyring. GPG looks at the
`GNUPGHOME` environment variable to see where to read its public and
private keys from. (On Linux-like systems this defaults to `~/.gnupg`
while on Windows it's stuffed away in the (possibly hidden) directories:

`C:\Documents and Settings\username\Application      Data\GnuPG`\
 or\
 `C:\Users\username\Application Data\GnuPG`\
 or\
 `C:\Users\username\AppData\Roaming\GnuPG`\

If you want to make multiple keyrings, set this environment variable
before running your gpg commands. (e.g. in a Linux shell,
`export GNUPGHOME=/directory/of/your/keyring` or in Windows,
`set GNUPGHOME=c:\directory\of\your\keyring` and then subsequent
commands in that shell will use your "sandbox" keyring.)

Note that gpg will check the permissions on that folder and operations
that call external programs (like connecting to a keyserver) will be
disallowed if others can write to that directory. In a Unix-like system,
you can fix that with:

`chmod 700 $GNUPGHOME`

For example, you can create a whole new keyring for automated processes:

`#!/bin/sh     export GNUPGHOME=/directory/of/your/keyring      # Following commands in this shell will use that home     gpg --import file1    `{.input}

Alternately, you can pass the `--homedir dir` option to gpg on the
command-line with each command.

### Forcing Different Algorithms

First, read the [Using Stronger Algorithms](#StrongerAlgorithms) section
above to see how to configure gpg to prefer that people use certain
algorithms when sending to you. That section is probably more important
than this one. It's far more important that you and the person you're
talking to use the recommendations in the [Using Stronger
Algorithms](#StrongerAlgorithms) section above.

GPG contains many different encryption and hashing algorithms. You can
get a list of the included algorithms with the command:

`gpg --version`{.input}\
\

`gpg (GnuPG) 1.4.13 Copyright (C) 2012 Free Software Foundation, Inc. License GPLv3+: GNU GPL version 3 or later <http://gnu.org/licenses/gpl.html> This is free software: you are free to change and redistribute it. There is NO WARRANTY, to the extent permitted by law.  Home: ~/.gnupg Supported algorithms: Pubkey: RSA, RSA-E, RSA-S, ELG-E, DSA Cipher: IDEA, 3DES, CAST5, BLOWFISH, AES, AES192, AES256, TWOFISH,         CAMELLIA128, CAMELLIA192, CAMELLIA256 Hash: MD5, SHA1, RIPEMD160, SHA256, SHA384, SHA512, SHA224 Compression: Uncompressed, ZIP, ZLIB, BZIP2`{.output}

When manually encrypting, (either with public-key encryption or
symmetric encryption,) you can specify an encryption algorithm with the
`--personal-cipher-preferences "alg1 alg2..."` option and a
digest/hashing algorithm using the
`--personal-digest-preferences "alg1 alg2..."` option:

`gpg --armor --personal-cipher-preferences "AES256     AES192 AES" --personal-digest-preferences "SHA512 SHA256 SHA1" -r     recipient1@email.address --encrypt filename`{.input}

You really need to know what you're doing to use these, though. See the
[GPG Protocol-Specific Options
page](http://www.gnupg.org/documentation/manuals/gnupg-devel/OpenPGP-Options.html)
for more.

**Expert tip:** If you really want to force the algorithm used, you can
use the `--cipher-algo name` command-line switch for symmetric or
public-key encryption. The `--personal-cipher-preferences` options above
should be used if you don't want to accidentally violate the OpenPGP
specification. You can use the `--cipher-algo name` argument if you know
that your recipient has a modern version of GPG but doesn't have their
public key set up well. Again, encourage them to improve their public
key using the [Using Stronger Algorithms](#StrongerAlgorithms) section
above.

### Protecting your Secret Keys

**Warning:** This section is somewhat speculative and may not help you
really improve your security against a sophisticated attacker, but may
help defeat some threat models.

Your secret keys are, by default, encrypted with older encryption
algorithms (CAST5) and hashing algorithms (SHA-1, iterated over 65,536
rounds). You can modify these preferences, though.

You must use a strong password to protect your secret keys. This is the
weakest link of your security. If someone is able to obtain your secret
key files, they can mount a brute-force attack on it by testing many
passwords in a dictionary attack. If you want to make it harder to
perform a naïve brute-force attack on your secret keys, you can change
the encryption algorithm and increase the number of rounds that are
necessary to decrypt and validate your secret key. One way of doing this
is to change the password for your secret key with something like the
following:

`gpg --interactive --s2k-cipher-algo AES256 --s2k-digest-algo SHA512 --s2k-mode 3 --s2k-count 65000000 --edit-key keyID`

and then changing the password using the `passwd` command,
saving/quitting using `save` and saving the changes.

This forces your secret key to be encrypted with the AES-256 algorithm,
SHA-512 hashing, and the mode is iterated and salted. The count means
that the hash will be applied 65 million times (which is about the
maximum allowed.) This will greatly slow down the decryption of your
secret key (it takes about a second on my computer, but that's rarely a
problem,) which might significantly slow down attackers attempting to
brute-force your password. Reduce the count if you need to decrypt many
messages very quickly, as you will encounter a noticeable delay every
time you decrypt a message!

**Technical Note:** `s2k` is short for "string to key". This refers to
an algorithm that turns a textual string (*i.e.* your password) into an
*n*-bit number that can be used as a cryptographic key. (For example,
AES-256 requires a 256-bit-long key. Your password is probably not that
long, nor evenly distributed bitwise, so these functions try to turn a
shorter string into a well-distributed longer key.)

The more expensive that you make attacks on your secret keys, the
better. This may not protect you against the highest-level attackers,
nor will it prevent attacks directly against the symmetrically-encrypted
parts of your message (see the [Using Stronger
Algorithms](#StrongerAlgorithms) section above to improve this,) but it
will certainly discourage someone who has obtained your secret keyring
and is trying to brute-force the password (say, by using the
password-generating features of [John the
Ripper](http://www.openwall.com/john/) and passing them into the GPG
executable.) This will slow down the speed of password cracking by many
orders of magnitude, which is often enough to make brute-force attacks
greatly infeasible.

More information at Christopher Wellons's excellent [blog
entry](http://nullprogram.com/blog/2012/06/24/).

In the OpenPGP standard, the number of iterations is actually coerced
into a single byte, so not all numbers of iterations are possible.
Here's more information about the [equation and valid
values](http://www.reddit.com/r/GnuPG/comments/21njsb/s2kcount_illegal_numbers/)
for `--s2k-count`.

There is [some
dispute](http://security.stackexchange.com/questions/15632/what-is-purpose-of-s2k-gnupg-options)
if these particular options are the best, so do your research. For
example, AES algorithms are designed to be fast, so a slower algorithm
might actually be better if you're trying to slow down attackers.

It is also possible that this could *weaken* your security if the
hashing algorithm has fixed points or cycles, that is, values where the
input to the hashing function equals the output from the hashing
function. Extending the number of iterations may make it *more* likely
that a fixed point or cycle is struck. (Read Donald Knuth's amusing
anecdote about fixed points in his homemade random number generator in
Volume 2 of *The Art of Computer Programming* about how easy it can be
to strike fixed points. *(Legal links, anyone?)*) More research is
warranted. **Update:** I did more research in the technical note below.

**Technical Note:** I decided to do the math on this, to estimate the
probability of a hash cycle or collision with highly-iterated hashing.
If we can assume that the output of the hash function is approximately
random with respect to the input, (that's a rather strong assumption,)
the mathematics of the problem reduce to an analog to the [Birthday
Problem](https://en.wikipedia.org/wiki/Birthday_problem) (that is, the
probability that at least one birthday is shared by at least 2 people in
of a group of `n` people.)

The probability `p` of a cycle with `n` iterations and `states` states
in the hash function can be estimated by:

`p(n, states) = 1 - e(-n)(n-1)/(2 * states)`{.input}

Since the argument of the exponent is often a very small number, due to
the number of states being very high, (2^128^ for MD5, 2^160^ for SHA-1,
2^512^ for SHA-512,) we will have to use an arbitrary-precision
exponential function and extended precision in many environments. Below
is a [Frink](http://futureboy.us/frinkdocs/) program (a programming
language that I wrote) that calculates the probabilities.

`use ArbitraryPrecision.frink      setPrecision[200]      p[n, states] := 1 - arbitraryExp[((-n)(n-1)/(2 * states))]     `{.input}

This function can then be called as follows (for the SHA-1 function with
2^160^ states and 65 million iterations):

`p[65 million, 2^160]`{.input}\
 `1.445e-33`{.output}\

Thus, we can derive the following probabilities of hitting a cycle in
various hash functions, *assuming* they're close to random:

Hash Function

Bits

Bytes

Cycle probability in 65 million iterations

MD5

128

16

6.2\*10^-24^

SHA-1

160

20

1.4\*10^-33^

SHA-224

224

28

7.8\*10^-53^

SHA-256

256

32

1.8\*10^-62^

SHA-384

384

48

5.4\*10^-101^

SHA-512

512

64

1.6\*10^-139^

Thus, the probability of seeing a random hash cycle with the SHA-512
procedure above are so low (given our assumptions!) that we can estimate
that it won't happen in the lifetime of anyone on the planet living
today, and we can proably safely assume that using many iterations, as
noted above, will probably improve our security. *QED.*

*Note:* I'm also running homemade programs that are attempting to find
cycles in iterated MD5 hashes. It builds a giant hash table of the last
100 million hashes it has seen, and will detect any cycle shorter than
this. It's not likely I'll find one if the hashing function is designed
well.

### Backing Up Your Secret Key

If, for some reason, you want to back up your secret key and possibly
print it, you can use the `--export-secret-key --armor` option to `gpg`,
possibly using the `--output filename` option to output to a specified
file. Then you could, say, engrave that onto a piece of metal and store
it away in a cave for 1000 years. Or whatever. It will be ponderous and
error-prone to type that key back in, especially with a large key or a
key that contains a photo.

### "Creating the perfect GPG keypair"

**Warning:** Read this whole section before making any decision. This
section is actually a warning *against* these practices, rather than a
recommendation.

Alex Cabal has a document entitled ["Creating the perfect GPG
keypair"](https://alexcabal.com/creating-the-perfect-gpg-keypair/) (Link
opens in new window) in which he describes creating subkeys of your
keypair that you can use on a device like your laptop, which somewhat
mitigates the risk of your laptop being stolen. In short, it allows you
to create a new subkey that is used only for signing, which you keep on
that laptop. If the laptop is stolen, you can revoke that signing key
which is claimed to prevent the thief from impersonating you. However,
*I think that this practice is very dangerous, if not outright wrong.*
There are good tips about managing secret keys in this document, but I
argue against its primary premise.

You should be most strongly warned that these practices will leave your
communications wide open for interception. The document linked above
does not warn you *in the strongest possible terms* that the practice of
creating the "perfect key" lets whoever stole your laptop decrypt and
forever continue to decrypt all your email (if they can guess the
password used to encrypt your secret key) yet you go on blithely
pretending they can't! That is very poor practice. All that the subkey
business does is prevent the attacker from *impersonating* you by
signing messages. (But, again, *only* if they can guess the password
used to encrypt your secret key, and only if your recipients know that
you've revoked the key.) If they can guess your password, the attacker
could still read *all* your encrypted messages *forever*. Read on.

Unless everyone that you communicate with *regularly* does something
like:

`gpg --refresh-keys`{.input}

to find out that keys have been revoked, they may never even *know* that
you revoked the signing key, and they will continue to trust your
signature.

If the person who stole your laptop (and thus your secret keys) could
*ever* impersonate you (because they guessed the password for your
secret key), then they can *forever* decrypt all the communications sent
to you with that same key if you follow the "perfect keypair" advice.

Allowing your attacker to read your encrypted communications forever,
and pretending it didn't happen, is extremely bad and wrong
cryptographic practice, obviously. If your decryption key is stolen,
*revoke that entire keypair and never use any part of it again*!
Otherwise, your attacker can forever read messages encrypted to your
public key.

It appears that the primary benefit of following this procedure is not
having to rebuild your web of trust with a new key. However, how much
trust should you give to someone who still uses a key that has been
knowingly compromised and does not properly protect your communications
with them? The answer is none. None more trust.

### OpenPGP Specification

For details on the public OpenPGP specification, see [RFC
4880](https://tools.ietf.org/html/rfc4880).

* * * * *

This page is a perpetual work-in-progress. If you have questions,
corrections, suggestions, tool suggestions, or want to exchange
encrypted e-mails, please contact [Alan
Eliasen](mailto:eliasen@mindspring.com) or on Twitter as
[@aeliasen](https://twitter.com/aeliasen). Thanks!

[Back to home page.](/)
