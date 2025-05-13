---
layout: wrapper
title: Introduction
permalink: /introduction/
---
<hr>
<br>
<div>
    <h3>About the Project</h3>
    <div>
        <h4>North American Bird Migration Analysis (1970s vs. 2010s)</h4>
        <div class="quote-box">
            <p>"<span class="quote">Birds are indicators of environmental health for their own species, people, and other wildlife.</span>" - Dayer, associate professor in the Department of Fish and Wildlife Conservation at Virginia Tech (Ashburn, 2024).</p>
        </div>
        <p>Experts say that recent data suggests bird populations in North America have seen a loss of more than 1 in 4 birds since 1970. That's approximatelt 2.9 billion birds, a finding from the first-ever comprehensible assessment of the net population changes of birds in the United States and Canada (Cornell Lab, 2019). Some of the major reasons for this include, but is not limited to, habitat loss caused by agricultural intensification, urbinization, and climate change. 1 billion birds are shown to due each year due to collision with windows, a direct result of increased urbanization (Ashburn, 2024).</p>
        <p>This trend is happening amongst birds in every biome. Forest birds have seen a decline of 1 billion birds. Grassland birds have collectively declined around 53% or 720 million birds. What's more, the greatest losses are seen amongst the most common birds, from popular sights in bird feeders such as white-throated sparrows, to common sightings in nature, such as the red-winged blackbird. More than 90% if the overall losses are from jsut 12 families of common species, including sparrows, blackbirds, warblers, and finches (Cornell lab, 2019).</p>
        <p>As such, this project aims to see if <span style="font-weight: bold">bird migration patterns in North America</span> between the <span style="font-weight: bold">1970s and the 2010s</span>, using data collected from the <a href="https://www.sciencebase.gov/catalog/item/653fa806d34ee4b6e05bc57d">U.S. Geological Survey ScienceBase Catalog</a> will show us a similar story, determining if bird banding is a useful tool in the analysis of bird trends caused by external factors such as agriculture expansion, urbanization, and climate change.</p>
    </div>
    <div>
        <h4>Focus Species</h4>
        <p>We focus on <span style="font-weight: bold">seven bird species</span> selected for their diversity, abundance of records, and their grouping within the dataset:</p>
        <ul>
            <li>Canada Goose</li>
            <li>Wood Duck</li>
            <li>Mourning Dove</li>
            <li>Tree Swallow</li>
            <li>Gray Catbird</li>
            <li>American Goldfinch</li>
            <li>White-throated Sparrow</li>
        </ul>
        <p>To streamline the analysis, we retained only the data from <span style="font-weight: bold">1970 and 2010</span>, allowing for a clear comparison of migration patterns across these two decades. Each specie family in the dataset encompassed several species, so to main bias and to get a more streamlined overview, we chose to focus on one species from each family. Each of the chosen species furthermore has a good amount of data for analysis.</p>
    </div>
    <div>
        <h4>Objectives</h4>
        <ul>
            <li>Understand how <span style="font-weight: bold">migration patterns have changed</span> temporally and geographically.</li>
            <li>Identify <span style="font-weight: bold">the number of birds banded</span>, <span style="font-weight: bold">the banding events</span>, and their <span style="font-weight: bold">subdivisions</span>.</li>
            <li>Compare patterns and trends between the <span style="font-weight: bold">1970s and 2010s</span>.</li>
        </ul>
    </div>
    <div>
        <h4>Importance of Bird Banding</h4>
        <p><span class="italic">The North American Bird Banding Program (NABBP)</span>, administered by the <span class="italic">U.S. Geological Survey (USGS) Bird Banding Laboratory</span> and the <span class="italic">Canadian Wildlife Service's Bird Banding Office</span>, uses standardized event types to categorize different bird banding activities.</p>
        <p>For some context, bird banding in North America was first introduced in 1803 by John James Audubon, who tied silver wire around the legs of nestling eastern phoebes, two of which returned the following spring. Later on in 1882 Ernest Thompson Seton used printer's ink to mark snow buntings. In 1996, the North American Banding Council (NABC) was formed. Their mission was to train banders in safe, ethical practices of the capture and handling of wild birds.</p>
        <p>Studies of bird migration are crucial. Modern bird banding efforts support:</p>
        <ul>
            <li>Research on avian behavior, ecology, and population dynamics</li>
            <li>Conservation of endangered species</li>
            <li>Regulation of hunting** for game birds</li>
            <li>Human health and safety initiatives (e.g., monitoring West Nile virus, preventing bird strikes near airports)</li>
        </ul>
        <p>Results from banding activities also contribute to international conservation programs such as:</p>
        <ul>
            <li>Partners in Flight</li>
            <li>North American Waterfowl Management Plan</li>
        </ul>
        <p>For more details, see the <a href="https://en.wikipedia.org/wiki/North_American_Bird_Banding_Program">North American Bird Banding Program - Wikipedia</a>.</p>
    </div>
</div>
<div>
    <h3>Introductory statistics</h3>
    <div>
        <h4>Data Cleaning</h4>
        <p>To begin with data collection we used 7 csv files from <a href="https://www.sciencebase.gov/catalog/item/653fa806d34ee4b6e05bc57d" target="_blank">ScienceBase</a>, which include data from 1970 to 2023. To reduce the data size, we focused on the 1970s and 2010s decennies and 7 focus species. As part of the cleaning process, we dropped duplicates and chose to keep data entries with less than 20% missing values. It should be noted we kept data entries with null values in features we will not be looking at, such as age. The "event date" and "band type" features, which we primarily focus on, are both cleaned for analysis.</p>
    </div>
    <div>
        <h4>Overall Bird Distribution Changes from 1970s to 2010s</h4>
        <p class="italic">The graph below is interactive. You can highlight each decade by clicking on the name in the legend.</p>
        <iframe src="/assets/intro/bird_banding_by_species_and_decade3.html" width="700" height="600" frameborder="0"></iframe>
        <p>The dataset contains 7 species with 23 features. Among the 7 species Canada Goose is the highest population with (1284279) and least bird is Tree Swallow. NABBP conducted 2 types of events B:Banding and E: Encounter where B indicates the initial banding event, where a bird is captured and a band is applied for the first time, E: Encounter represents a subsequent encounter with a previously banded bird. Encounters can occur through various means, such as recapture, resighting, or recovery. To band the species they used 25 different band types used based on their gender, age, size and location,among those band type 11 and 41 band types are mostly banded. Year with most bird band events conducted: 1971. with Count: 299230 Year with fewest bird band events: 1977 with Count: 175587. The most migrated countries are United States (US) and Canada (CA) in given period. Bird baded events are conducted several locations and they grouped to become a subdivions. The highest bird banded events conducted in Canada in Ontarion (CA-ON) and in US is New York (NY).Ontario is Canada's most populous province and a major location for bird banding activities due to its diverse habitats, including forests, wetlands, and large migratory corridors along the Great Lakes. New York is a key state for bird banding due to its strategic location along the Atlantic Flyway, a major migratory route for many bird species.</p>
    </div>
    <div>
        <h4>Overall Geographical Data</h4>
        <p class="italic">The map below is interactive. You can change what species to view by unchecking or checking in the rightside legend.</p>
        <iframe src="/assets/intro/interactive_species_banding_map_distinct_colors_clean.html" width="700" height="600" frameborder="0"></iframe>
        <p>Bird banded events are conducted several locations, Under one subdivions covers many locations with (LAT_DD and LOG_DD). The highest bird banded events conducted in Canada in Ontarion (CA-ON) and in US is New York (NY).Ontario is Canada's most populous province and a major location for bird banding activities due to its diverse habitats, including forests, wetlands, and large migratory corridors along the Great Lakes. New York is a key state for bird banding due to its strategic location along the Atlantic Flyway, a major migratory route for many bird species.</p>
    </div>
    <div>
        <h4>Example of temporal change between 1970s and 2010s</h4>
        <p class="italic">The graph below is interactive. You can highlight each species by selecting and deselecting them in the legend.</p>
        <iframe src="/assets/intro/temproal_changes_of_bird_banding_events2.html" width="700" height="600" frameborder="0"></iframe>
        <p>The bird banded events conducted rate changed each year which indicates the increased or decreased population of that specific specie. However the overal the bird count increased on avarage. The most birds were banded in 1971 with 299230 and the lowest number birds banded in 1977 with count of 175,587.</p>
    </div>
    <div>
        <h3>Summary</h3>
        <p>Bird banded events conducted by North American Bird Banding Program (NABBP) where it tag color band around bird's neck or to legs according to their age, weight, gender, sepecies family to identify them in migration process. In this we focued on seven north amrican birds to analyse their migration patterns, geographical changes, temporal changes of the bird band events conducted in 1970 ans 2010s . Among the 7 species Canada Goose is the highly banded bird in selected period.</p>
    </div>


</div>