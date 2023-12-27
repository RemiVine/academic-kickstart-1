---
# Course title, summary, and position.
linktitle: Allocation algorithm grouping students
title: Allocation algorithm
toc: false
summary: An allocation algorithm to assign students to groups based on their preferences
weight: 1

# Page metadata.
# title: The Template
# date: "2018-09-09T00:00:00Z"
# lastmod: "2018-09-09T00:00:00Z"
# draft: false  # Is this a draft? true/false
# toc: false  # Show table of contents? true/false
# type: docs  # Do not modify.

# Add menu entry to sidebar.
# - name: Declare this menu item as a parent with ID `name`.
# - weight: Position of link in menu.
# menu:
#  example:
#    name: The template TEST
#    weight: 1

links: 
# - name: Slides
#  url: https://www.dropbox.com/s/yff0zuihe49szfp/Cata_Presentation.pdf?dl=0
url_pdf: './Thesis_template_RV.pdf'
# url_project: ''
# url_slides: '#'
# url_source: '#'
# url_video: '#'
# - icon: far fa-file-pdf
#  icon_pack: fa
#  url: img/Family_Migration_Africa_and_Europe_RV_JMP_last_version.pdf
# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/s9CC2SKySJM)'
  focal_point: ""
  preview_only: false


---


The algorithm with details and the example with the data used can be found: [here](https://github.com/RemiVine/Allocation_algorithm_ARP_GGI/blob/Allocation_algorithm/The_Algorithm.ipynb)

# Your Markdown content here...

```python
# Example Python code
def allocate_students(preferences):
    # Your allocation algorithm implementation
    pass

preferences = {
    'Alice': ['Group 1', 'Group 3', 'Group 5'],
    'Bob': ['Group 2', 'Group 4'],
    # ...other students and their preferences...
}

allocate_students(preferences)



```python
n = 10  # number of trials
x = list(range(n+1))  # list of values for x
y = [math.comb(n, i) for i in x]  # list of values for binomial coefficient
# plot
plt.plot(x, y, color='red', linewidth=1.5)
plt.xlabel('The size of the sample, n')
plt.ylabel('Number of possible different samples (Binomial Coefficient)')
plt.title('Number of possible different samples for N=10')
# save the plot as a PNG file
name_of_file = 'Number_combination_samples_for_sampling_distribution_N_10'
completeName = os.path.join(save_path, name_of_file+".png")         
plt.savefig(completeName)
# Show
plt.show()



