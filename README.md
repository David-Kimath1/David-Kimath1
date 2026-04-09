![Profile Views](https://komarev.com/ghpvc/?username=David-Kimath1)

// Cloudflare Worker script
export default {
  async fetch(request, env) {
    const url = new URL(request.url);
    const username = url.searchParams.get('username') || 'unknown';
    
    // Get or increment view count from KV store
    let views = await env.VIEWS.get(username);
    views = views ? parseInt(views) + 1 : 1;
    await env.VIEWS.put(username, views.toString());
    
    // Generate SVG with your animated code lines
    const svg = generateFuturisticSVG(views);
    
    return new Response(svg, {
      headers: {
        'Content-Type': 'image/svg+xml',
        'Cache-Control': 'no-cache'
      }
    });
  }
};

function generateFuturisticSVG(views) {
  // The SVG template from Option A, but with ${views} inserted dynamically
  return `<svg>...${views}...</svg>`;
}
