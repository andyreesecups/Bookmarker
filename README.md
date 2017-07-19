A bookmarker made with HTML, Boostrap, CSS, and Vanilla Javascript that allows users to bookmark their favorite websites. It stores their favorite websites in local storage. 


The code below uses regex to make sure the user inputs a correct url address in order for the bookmark to be saved. For example, if a user wants to visit www.atxdeveloper.com they must input http://www.atxdeveloper.com in order for it to work. If they do not input the correct url then an alert message pops up and says "Please use a valid URL".



  var expression = /[-a-zA-Z0-9@:%_\+.~#?&//=]{2,256}\.[a-z]{2,4}\b(\/[-a-zA-Z0-9@:%_\+.~#?&//=]*)?/gi;
  var regex = new RegExp(expression);

  if(!siteUrl.match(regex)){
    alert('Please use a valid URL');
    return false;
  }

  return true;
}


You can find this project at:  https://andyreesecups.github.io/Bookmarker/
