burnish.github.com
==================

Burnish Software website and blog.

## Instructions for future Philip

    > cat .ssh/config

    Host github.com-burnish
        HostName github.com
        User git
        IdentityFile ~/.ssh/id_rsa_burnish

    > git clone git@github.com-burnish:burnish/burnish.github.com.git
    > cd burnish.github.com

    # write the posts / do the edits

    > sudo gem install github-pages
    > bundle exec jekyll serve --watch # Check that it looks okay.
    > git push
