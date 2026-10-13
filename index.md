---
---

Data Carpentry aims to teach researchers basic concepts, skills, and tools 
for working
with data so they can get more done quickly and with less pain. This workshop uses 
Data Carpentry's approach to
teach data management and analysis for metagenomics research, including: 
best practices for the organization of bioinformatics projects and data, use
of command-line utilities, use of command-line tools to analyze sequence quality, 
use of R studio and use of R libraries to compare diversity between samples, 
and connecting to and using cloud computing. 
This workshop is designed to be taught over two full days of instruction.

Would you be interested in teaching these materials? We have an 
[Slack channel](https://join.slack.com/t/metagenomicslesson/shared_invite/zt-1tikq2o0k-VMX7ceLfenbbKheZ7XNCRw) 
were we will be happy to help you!


> ## Frequently Asked Questions
> Read our [FAQ](https://carpentries-lab.github.io/metagenomics-workshop/faq/index.html) to learn more about Data Carpentry's Metagenomics workshop as an Instructor or a workshop host.
{: .callout}

> ## Getting Started
>
> This lesson assumes that learners have no prior experience with the tools covered in the workshop.   
> 
> However, learners are expected to have some familiarity with biological concepts,
> including the 
> concept of DNA sequencing, nucleotide abbreviations, genome, microbiome, and taxonomy. Participants should bring their own laptops and plan to participate actively.  
> 
> To get started, follow the directions in the [Setup](https://carpentries-lab.github.io/metagenomics-workshop/setup.html) tab to 
> get access to the required software and data for this workshop.
>
> ### Logging in to ALICE
>
> If you are following this workshop on the ALICE HPC cluster of Leiden University, you
> work through the Open OnDemand web portal. The portal is not directly reachable from
> the internet, so first connect to the university network with eduVPN.
>
> 1. **Connect with eduVPN.** Install eduVPN (from the Company Portal on a managed laptop,
>    or from [eduvpn.org](https://www.eduvpn.org)), choose *Leiden University*, sign in with
>    your ULCN account, and make sure the connection is active.
>
>    <a href="{{ page.root }}/fig/alice_login_1_eduvpn.png">
>      <img src="{{ page.root }}/fig/alice_login_1_eduvpn.png" alt="eduVPN window showing an active connection to Leiden University" />
>    </a>
>
> 2. **Log in to the portal.** In your browser go to
>    [https://ood.alice.universiteitleiden.nl/](https://ood.alice.universiteitleiden.nl/)
>    and enter your ALICE username and password.
>
>    <a href="{{ page.root }}/fig/alice_login_2_ondemand.png">
>      <img src="{{ page.root }}/fig/alice_login_2_ondemand.png" alt="Open OnDemand login page asking for ALICE username and password" />
>    </a>
>
> 3. **Open a shell.** In the top menu choose *Clusters* > *ALICE Shell Access*.
>
>    <a href="{{ page.root }}/fig/alice_login_3_shell.png">
>      <img src="{{ page.root }}/fig/alice_login_3_shell.png" alt="ALICE OnDemand Clusters menu with ALICE Shell Access highlighted" />
>    </a>
>
> 4. **Change your password (first login only).** A terminal opens on a login node. The
>    first time, accept the host fingerprint by typing `yes`. If you received a temporary
>    password, type `passwd` at the prompt and follow the instructions to set a new one.
>
>    <a href="{{ page.root }}/fig/alice_login_4_password.png">
>      <img src="{{ page.root }}/fig/alice_login_4_password.png" alt="ALICE login node terminal with the passwd command typed at the prompt" />
>    </a>
>
> More details are in the
> [ALICE documentation](https://pubappslu.atlassian.net/wiki/spaces/HPCWIKI/pages/37749098/Accessing+ALICE+or+SHARK+with+a+web-browser+using+Open+OnDemand#For-ALICE-users).
> If eduVPN is not an option, you can instead connect to `nodelogin03` or `nodelogin04`
> via RDP and open the same address in Firefox there.
>
{: .prereq}

> ## Data
> 
> This workshop uses data from the environmental experiment: [Genomic adaptations in information 
> processing underpins trophic strategy in a whole-ecosystem nutrient 
> enrichment experiment](https://elifesciences.org/articles/49816), by Jordan G Okie et al.
> In this research, authors compared the differences between the microbial community 
> in its natural, oligotrophic, phosphorus-deficient 
>environment, a pond from the Cuatro Ciénegas Basin (CCB), and the same microbial 
>community under a fertilization treatment.
>
> All of the data used in this workshop can be downloaded from
> [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7010950.svg)](https://doi.org/10.5281/zenodo.7010950)
> More information about this data is available on the [Data page](https://carpentries-lab.github.io/metagenomics-workshop/data/index.html).
{: .prereq} 

# Workshop Overview 

| Lesson    | Overview | Estimated time|
| ------- | ---------- | ---------- |
| [Project Organization and Management](https://carpentries-incubator.github.io/organization-metagenomics/) | Learn how to structure your metadata, organize and document your metagenomics data and bioinformatics workflow, and access data on the NCBI sequence read archive (SRA) database.|1:30 hr|  
| [Introduction to the Command Line](https://carpentries-incubator.github.io/shell-metagenomics/) |  Learn to navigate your file system, create, copy, move, and remove files and directories, and automate repetitive tasks using scripts and wildcards. | 4:00 hr| 
|[Introduction to R](https://carpentries-incubator.github.io/introduction-to-R-for-metagenomics/) | Use R studio to manage several data types and structures. | 1:00 hr| 
|[Data Processing and Visualization for Metagenomics](https://carpentries-incubator.github.io/metagenomics/) | Use command-line tools to perform quality control, metagenomic assembly, metagenomic binning, taxonomic assignment, and diversity exploration. | 6:30 hr| 

<!--
# Optional Additional Lessons

| Lesson | Overview |
| ------- | -------- |
| [16S genomics](https://datacarpentry.org/genomics-r-intro/) | Use R to analyze and visualize between-sample variation. |
!-->

# Teaching Platform
This workshop is designed to be run on pre-imaged Amazon Web Services (AWS)
instances. All the software and data used in the workshop are hosted on an Amazon Machine Image (AMI).
If you want to run your instance of the server used for this workshop, follow the directions in the [Setup](setup.html) tab. 

## Citation
Please cite as:
[![DOI](https://jose.theoj.org/papers/10.21105/jose.00209/status.svg)](https://doi.org/10.21105/jose.00209)

Claudia Zirión Martínez; Diego Garfias Gallegos; Tania Vanessa Arellano Fernández; Aarón Espinosa Jaime; Edder D Bustos Díaz; José Abel Lovaco Flores; Luis Gerardo Tejero Gómez; J Abraham Avelar Rivas; Nelly Sélem (March , 2023) A Data Carpentry- Style Metagenomics Workshop

# Lessons Reference
The content of this page and three of the lessons presented in this workshop are adapted from lessons on the [Data Carpentry Genomics Workshop](https://datacarpentry.org/genomics-workshop/).
Lesson 1, Lesson 2, and Lesson 4, specifically Episode 2. Assessing Read Quality, and 3. Trimming and Filtering are adapted from the corresponding episodes in the [Data Wrangling and Processing for Genomics](https://datacarpentry.org/wrangling-genomics/) lesson that is Copyright (c) [The Carpentries](https://carpentries.org/). Materials licensed under [CC-BY 4.0](https://creativecommons.org/licenses/by/4.0/) by the authors: Josh Herr, Ming Tang, Lex Nederbragt, Fotis Psomopoulos (eds): Version 2017.11.0, November 2017. THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
