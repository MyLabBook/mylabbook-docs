# MyLabBook Blog

## Open Source Alternatives for an Electronic Lab Notebook
26 Oct 2009

According to some recent articles in the science technology press, ELNs are a growing market. For example, a 2006-2007 article at 
Scientific Computing estimated that the market was about 50 million USD in 2005 and was growing at 20% to 30% per year. 
This makes a great deal of sense when we take into account the growing complexity of science and the massive amount of data that is 
collected and needs to be analyzed. This is true especially in the life sciences, and several of the commercial ELN offerings are 
targeted primarily at that market (e.g., CERF by Rescentris, Inc.).

What does this mean for non-commercial ELNs, however? And what does it mean for academic institutions who desire to prepare their 
students for a future where ELNs will be more and more common place? Of course, it is obvious from this website where we think at 
least one good solution to these questions lie. But let's take a step back and see why we have chosen the particular solution that is 
presented on this website. What are the alternatives? What are the criteria to use in developing an ELN appropriate for an academic setting?

### What are the criteria to use in developing an ELN appropriate for an academic setting?

Let's tackle the last question first and then see what kind of alternatives can satisfy our criteria. Some of the main criteria are as follows.

1. Cheap or preferably free - because most academic institutions are constrained by budgets and would have difficulty justifying spending much 
money on an ELN for students
1. Able to be customized for different scientific or technical contexts - the nature of scientific experiments is that although there are some commonalities, it would be advantageous for an ELN to be adaptable enough to provide differences for, say, physics experiments versus biology experiments versus mathematical simulations
1. Open source and supported by a viable community - this is a variation on the first point, but if the ELN is open source, then it is usually free. This makes it also much easier to justify with a funding agency because of the minimal cost and the likelihood that research funds will result in a contribution back to the community. Ideally, a viable community is also present, which will imply continuity regardless of whether one person contributes or not in the future.
1. Social networking capabilities would be nice - with today's students becoming more and more in tune with social networking sites like Facebook and mySpace, it would be advantageous to utilize these capabilities in an ELN as well.
1. Fairly easy to set up, maintain and extend - while not strictly necessary, the easier it is to set up (everything else being equivalent), then the more widespread that we can expect the adoption of such a platform.

So using these criteria, we can narrow our choices. Criteria 3 suggests that the choice should be a popular open source platform. 
Criteria 4 suggests that it should run primarily on the web versus on the desktop. And criteria 2 suggests that it be fairly mature or 
robust so that people will have developed add-on components that can be re-purposed for scientific purposes. Criteria 5 suggests the use 
of a scripting language versus the use of Java, C or C++, at least for the mainstream of web developers.

* Django - web framework based on the Python scripting language
* Plone - web content management system (CMS) based on the Python scripting language
* Joomla - web CMS based on the PHP scripting language
* Ruby on Rails - web CMS based on the Ruby scripting language
* Drupal - web CMS based on the PHP scripting language

Ruby on Rails has the advantage of being written in Ruby, which is a relatively elegant scripting language and growing in its use. 
The framework itself lends to great productivity as well because of its standardized approaches. The myExperiment project has taken this approach.

Django has the advantage of being written in Python, which is also a relatively elegant scripting language with an even larger support 
community than has Ruby. It also shows itself to run at about twice the speed of Ruby or PHP and can be run simply on the desktop as well 
as the web in a straightforward manner. There are also numerous Python modules written for scientific purposes on the desktop that can be 
repurposed for the web as needed. However, Django itself is a web framework instead of a CMS. And for the CMS platforms built upon Django, 
then there do not seem to yet be a mature set of modules available "out of the box" for many capabilities.

Plone is probably the most mature of the CMS platforms built with Python, and is relatively easy to set up as long as one has full access to 
server configurations. However, like Django, it is not as widely supported by internet service providers and thus becomes less available in many cases.

Joomla is a popular web framework also, and has thousands of add-on modules and some very nice looking templates available.

In the end, though, we chose Drupal because of the following reasons.

The elegance of Drupal's architecture - while the PHP scripting language is not very elegant as compared to Python or Ruby, the Drupal architecture 
is very elegant and flexible. The structure is very well thought out and lends itself to tremendous flexibility.
Incorporation of the Semantic Web technologies - Drupal has been the first of the popular web platforms to incorporate Semantic Web technologies 
on a wide scale. These technologies are being incorporated into the core in the upcoming version 7 of Drupal, and have been available as modules 
for version 6 for some time. This approach holds tremendous potential for scientific communication and research. We believe that someday in the 
future, perhaps the not too distant future, that Semantic Web capabilities will be expected for an ELN. With Drupal, we will be getting this 
"out of the box", so to speak, before anyone else.
Breadth of available modules - as is documented in other areas on this site, the number of possible Drupal modules for an ELN is outstanding, 
ranging from plotting to spreadsheets to Google maps and many, many more. While Joomla may have some more mature modules in certain areas, 
they are often commercial as well, unlike Drupal. And Drupal seems to have a wider overall breadth of modules available.
Practical reasons - then we have the very practical reasons that the primary developer of this ELN is familiar with the PHP scripting language 
and with the Drupal platform. So that minimizes the learning curve for this approach and helps us to roll things out more quickly and easily. 
This is not a definitive reason, but given the other advantages, it gives us cause enough not to look further.
So that is some of the reasoning that went into the choice of the Drupal platform for our ELN. We continue to be happy with the choice, 
but also are interested in any feedback, pro or con.




