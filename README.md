<a href="https://models.svilenkovic.rs/"><img src="media/cover.jpg" alt="FOX Models, home page on a laptop and a phone" width="100%"></a>

# FOX Models

Redesign of a Belgrade modeling agency's website: boards, model profiles with measurements, editorials and a new faces application.

**[models.svilenkovic.rs](https://models.svilenkovic.rs/)** · [Case study (in Serbian)](https://svilenkovic.com/radovi/fox-models) · [Srpski](README.sr.md)

> [!NOTE]
> Client project. The source code belongs to the client and stays in a private repository. This page describes what I built and how.

<table>
  <tr><td><b>Client</b></td><td>FOX Models</td></tr>
  <tr><td><b>Industry</b></td><td>Modeling agency</td></tr>
  <tr><td><b>Location</b></td><td>Belgrade, Serbia</td></tr>
  <tr><td><b>Type</b></td><td>Multi-page website</td></tr>
  <tr><td><b>My role</b></td><td>Redesign, design, development and SEO</td></tr>
  <tr><td><b>Stack</b></td><td>HTML, CSS, vanilla JS, nginx</td></tr>
</table>

## About the project

FOX Models is a Belgrade modeling agency with a women's and a men's board, scouting, and work for fashion houses, magazines and brands, and I am redesigning its website. On a site like this the photo is the product, so everything else has to stay out of its way. An earlier dark version had a 3D photo ring; this light one without any 3D got all the later revisions and a much simpler home page. The working version runs on my subdomain, closed to indexing, while the agency's current site stays on foxmodel.com.

I wrote it in plain HTML, CSS and JavaScript, with no framework and no build step, about 70 KB of my own code in three files. The data file uses the same fields as the columns an agency database would return, one row per model, so a real database can replace the demo data without touching the site. Updating content means copying one file to the server, while the 3D version, a Next.js project, had to be rebuilt.

## What I built

- A split home page: W on the left for the women's board, M on the right for the men's, and the M is the same W turned upside down
- Boards with Main, New Faces and Commercial tabs, live search by name and an A to Z index with Serbian letters that appears from twelve models up
- A profile with its own URL and measurements for every model, and a booking link that opens a pre-filled email
- An editorials wall with a lightbox that works by keyboard and by swipe and keeps focus inside while open
- A fix for a redirect that dropped the query string, which had made every profile open the first model on the list
- Separate cache rules: CSS, JS and HTML always revalidate, images stay cached for seven days

## Screenshots

<table>
  <tr>
    <td width="68%" valign="top"><img src="media/desktop.webp" alt="FOX Models, home page on a 1440 px screen"></td>
    <td width="32%" valign="top"><img src="media/mobile.webp" alt="FOX Models, home page on a phone"></td>
  </tr>
</table>

<img src="media/inner-1.webp" alt="The &quot;Izdvojeni&quot; (Featured) section: four faces from the women's board and four from the men's board">
<sub>The "Izdvojeni" (Featured) section: four faces from the women's board and four from the men's board</sub>

<img src="media/inner-2.webp" alt="Footer: boards, the agency and separate contact addresses for booking and scouting">
<sub>Footer: boards, the agency and separate contact addresses for booking and scouting</sub>

---

<sub>Built by [D. Svilenković](https://svilenkovic.com).</sub>
