# NextJS tutorial - React foundations

The tutorial can be found at: [https://nextjs.org/learn/react-foundations](https://nextjs.org/learn/react-foundations)

![9/9 Completed](nextjs-react-foundations.png)

## Custom config for Github pages deploy

```js
// Chapter-09_Installing Next.js/next.config.js
/**
 * @type {import('next').NextConfig}
 */
const nextConfig = {
    output: 'export',

    distDir: '../docs',
    assetPrefix: '/nextjs-react-foundations/',
}

module.exports = nextConfig
```

### :monocle_face: Take care

Remember to put an empty file .nojeyll named in the output folder or Github will ignore all the js files in _next folder

```js
// Chapter-09_Installing Next.js/package.json
{
  "scripts": {
    "dev": "next dev",
    "build": "next build && touch ../docs/.nojekyll"
  },
  "dependencies": {
    "next": "^14.0.1",
    "react": "^18.2.0",
    "react-dom": "^18.2.0"
  }
```


## Credits

NextJS.org - tutorial
[https://nextjs.org/learn/react-foundations](https://nextjs.org/learn/react-foundations)

This README has been optimized for accessibility based on GitHub's blogpost "[Tips for Making your GitHub Profile Page Accessible](https://github.blog/2023-10-26-5-tips-for-making-your-github-profile-page-accessible)"

## License

[MIT](https://github.com/nervaccio/nextjs-react-foundations/blob/main/LICENSE)
