---
title: "Network Link Prediction"
date: 2022-04-01
image: "images/portfolio/item-5.png"
project_url : "https://github.com/lonewolf045/social-network-link-prediction"
categories: ["ML"]
description: "Social Network Link Prediction"
draft: false
---

#### Project Details

This was a group Project, undertaken in requirement for the BTech degree.   

Stated simply, the task of link prediction is to predict whether a relationship (or an edge) can exist between two nodes in a given network.  
Most existing methods for doing so exploit the network structure or attributes of nodes and edges in the network. Two broad paradigms exist for the same, GNN based encodings and Structure based encodings of nodes. In our work, we explored how the two encodings perform on the task of link prediction and compare the results of using one against the other and also, a combination of the two.  

A total of four datasets from the Stanford Network Analysis Project (SNAP) were considered, which contain various kinds of relationships between users of online platforms. The datasets used are:  
* Epinions Social Network : This is a trust-based, medium-sized social network, used by several other related works for a variety of tasks. An edge in the Epinions network represents a relationship in which a user chooses to trust another based on the latter’s published reviews on the website.  
* GitHub Social Network : This network provides information on "follow” relationships between users having a minimum of 10 starred repositories.  
* Wikipedia Vote Network : This is a network that contains data about voting pertaining to Request for Adminship (RfA) on Wikipedia.  
* Twitch Social Networks : These represent friendships between gamers who stream in a certain language, with there being a separate sub-network for each such language.  

Experimented using node representations with ensemble ML models and empirically tried neural network architectures for predicting links on 4 different social network datasets.  
Finally, proposed a combination of learned representations and heuristics. Demonstrated improvements in F1 score across most datasets and predictive modelling techniques using this new feature set.  

[Preprint](https://drive.google.com/file/d/1fSQrkQXJer_B1ZuoHBgKkTpEBXpfH258/view?usp=sharing)  

Our work got accepted to the MAISoN workshop of the [IJCAI 2023](https://2023.maisonworkshop.org/accepted-papers)!  

I presented at the workshop, [here](https://drive.google.com/file/d/1zZTemQ5n1ks1w0PabGAkKA0is6r59MXO/view?usp=sharing) is the recording.  
