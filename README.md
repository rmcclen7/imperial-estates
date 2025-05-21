# imperial-estates
imperial estates realty listings 
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Imperial Estates Listings</title>
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600&display=swap" rel="stylesheet">
  <style>
    body {
      font-family: 'Montserrat', sans-serif;
      margin: 0;
      padding: 20px;
      background: #f9f9f9;
      color: #333;
    }

    .filter-bar {
      background: #fff;
      box-shadow: 0 2px 8px rgba(0, 0, 0, 0.07);
      margin-bottom: 40px;
      padding: 20px;
      border-radius: 8px;
    }

    .filter-bar input,
    .filter-bar select {
      padding: 10px 14px;
      border: 1px solid #ccc;
      border-radius: 6px;
      font-size: 14px;
      width: 100%;
      max-width: 220px;
      margin: 5px;
    }

    .filter-bar select:focus,
    .filter-bar input:focus {
      outline: none;
      border-color: #0b2545;
      box-shadow: 0 0 0 2px rgba(11, 37, 69, 0.2);
    }

    .filter-bar button {
      background-color: #0b2545;
      color: #fff;
      padding: 10px 18px;
      border: none;
      border-radius: 6px;
      cursor: pointer;
      margin: 5px;
      font-weight: 600;
      transition: background-color 0.3s ease;
    }

    .filter-bar button:hover {
      background-color: #081b35;
    }

    .listing {
      display: flex;
      flex-wrap: wrap;
      background: #ffffff;
      margin-bottom: 30px;
      border: 1px solid #ddd;
      border-radius: 8px;
      box-shadow: 0 2px 5px rgba(0, 0, 0, 0.05);
    }

    .listing img {
      width: 100%;
      max-width: 500px;
      border-right: 1px solid #ddd;
      object-fit: cover;
      border-radius: 8px 0 0 8px;
    }

    .info {
      flex: 1;
      padding: 20px;
      background: #fcfcfc;
    }

    .info h2 {
      margin-top: 0;
      font-size: 22px;
      color: #0b2545;
      font-weight: 600;
    }

    .info p {
      margin: 8px 0;
      line-height: 1.6;
      font-size: 15px;
      color: #444;
    }

    .button {
      background: #b68d40;
      color: white;
      padding: 10px 16px;
      text-decoration: none;
      border-radius: 4px;
      display: inline-block;
      margin-top: 15px;
      font-weight: bold;
      transition: background 0.3s ease;
    }

    .button:hover {
      background: #9d7935;
    }
  </style>
</head>

<body>

  <!-- Search and Filter Bar -->
  <div class="filter-bar">
    <div style="display: flex; flex-wrap: wrap; justify-content: space-between; align-items: center; gap: 10px;">
      <input type="text" id="searchInput" placeholder="Search by location, price, features...">

      <select id="priceFilter">
        <option>Price Range</option>
        <option>$100k - $300k</option>
        <option>$300k - $500k</option>
        <option>$500k+</option>
      </select>

      <select id="bedFilter">
        <option>Bedrooms</option>
        <option>1+</option>
        <option>2+</option>
        <option>3+</option>
        <option>4+</option>
      </select>

      <select id="typeFilter">
        <option>Property Type</option>
        <option>House</option>
        <option>Land</option>
        <option>New Construction</option>
      </select>

      <button id="filterBtn">Filter</button>
    </div>
  </div>

  <!-- Example Listing -->
  <div class="listing" data-price="744900" data-beds="5" data-type="House">
    <img src="https://photos.zillowstatic.com/fp/f6688c5f74d2b2c59faad4ab60db212a-cc_ft_1536.webp" alt="87 Marcus Ct">
    <div class="info">
      <h2>87 Marcus Ct, Ball Ground, GA 30107</h2>
      <p><strong>MLS #:</strong> 415767</p>
      <p><strong>Price:</strong> $744,900</p>
      <p><strong>Specs:</strong> 5 Beds | 4.5 Baths | 5,307 sqft | Built 2005</p>
      <p>Nestled on 3 private wooded acres, this home backs to a protected nature preserve. Chef’s kitchen, finished terrace level, and no HOA.</p>
      <a href="https://www.zillow.com/homedetails/87-Marcus-Ct-Ball-Ground-GA-30107/227636354_zpid/" target="_blank" class="button">Schedule a Viewing</a>
    </div>
  </div>

  <div class="listing" data-price="319000" data-beds="3" data-type="New Construction">
    <img src="https://photos.zillowstatic.com/fp/f6d7050e3dea1f599434f05cce3c9bba-uncropped_scaled_within_1344_1008.webp" alt="71 Hood Park Ct">
    <div class="info">
      <h2>71 Hood Park Ct, Jasper, GA 30143</h2>
      <p><strong>MLS #:</strong> 415768</p>
      <p><strong>Price:</strong> $319,000</p>
      <p><strong>Specs:</strong> 3 Beds | 2.5 Baths | 1,576 sqft | Built 2022</p>
      <p>Craftsman in Hood Villas with open floor plan, granite kitchen, spa-like primary suite, and stubbed basement. Close to downtown Jasper.</p>
      <a href="https://www.zillow.com/homedetails/71-Hood-Park-Ct-Jasper-GA-30143/82471025_zpid/" target="_blank" class="button">Schedule a Viewing</a>
    </div>
  </div>

  <div class="listing" data-price="329000" data-beds="4" data-type="New Construction">
    <img src="https://photos.zillowstatic.com/fp/41664c221ca90f7de47db86e2706ff69-uncropped_scaled_within_1344_1008.webp" alt="28 Hood Park Ct">
    <div class="info">
      <h2>28 Hood Park Ct, Jasper, GA 30143</h2>
      <p><strong>MLS #:</strong> 408374</p>
      <p><strong>Price:</strong> $329,000</p>
      <p><strong>Specs:</strong> 4 Beds | 3.5 Baths | 1,580 sqft | Built 2022</p>
      <p>Rare 4-bedroom plan with dual owner’s suites, open living, crown molding, and a spacious kitchen island. Ideal for families and entertaining.</p>
      <a href="https://www.zillow.com/homedetails/28-Hood-Park-Ct-Jasper-GA-30143/82440571_zpid/" target="_blank" class="button">Schedule a Viewing</a>
    </div>
  </div>

  <div class="listing" data-price="289200" data-beds="3" data-type="New Construction">
    <img src="https://photos.zillowstatic.com/fp/a81d2fb1b0def833d80bf690b1bdd4a6-uncropped_scaled_within_1344_1008.webp" alt="160 Pinto Ln SE">
    <div class="info">
      <h2>160 Pinto Ln SE, Fairmount, GA 30139</h2>
      <p><strong>MLS #:</strong> 401188</p>
      <p><strong>Price:</strong> $289,200</p>
      <p><strong>Specs:</strong> 3 Beds | 2.5 Baths | 1,419 sqft | Built 2024</p>
      <p>Brand new construction in Mustang Ridge! Two-story layout with open living, walk-in closets, premium finishes, and a quiet cul-de-sac location near Cartersville.</p>
      <a href="https://www.zillow.com/homedetails/160-Pinto-Ln-SE-Fairmount-GA-30139/444000285_zpid/" target="_blank" class="button">Schedule a Viewing</a>
    </div>
  </div>

  <div class="listing" data-price="292000" data-beds="3" data-type="New Construction">
    <img src="https://photos.zillowstatic.com/fp/784141d70c79df194b75f478dec7d866-uncropped_scaled_within_1344_1008.webp" alt="157 Pinto Ln SE">
    <div class="info">
      <h2>157 Pinto Ln SE, Fairmount, GA 30139</h2>
      <p><strong>MLS #:</strong> 401189</p>
      <p><strong>Price:</strong> $292,000</p>
      <p><strong>Specs:</strong> 3 Beds | 2.5 Baths | 1,419 sqft | Built 2024</p>
      <p>Charming two-story in Mustang Ridge featuring premium finishes, open-concept main level, spacious closets, and convenient access to Fairmount and Cartersville.</p>
      <a href="https://www.zillow.com/homedetails/157-Pinto-Ln-SE-Fairmount-GA-30139/442730379_zpid/" target="_blank" class="button">Schedule a Viewing</a>
    </div>
  </div>

  <div class="listing" data-price="299200" data-beds="3" data-type="New Construction">
    <img src="https://photos.zillowstatic.com/fp/69563d8bc9a698f79cc59215f4ddfdb6-uncropped_scaled_within_1344_1008.webp" alt="142 Pinto Ln SE">
    <div class="info">
      <h2>142 Pinto Ln SE, Fairmount, GA 30139</h2>
      <p><strong>MLS #:</strong> 401186</p>
      <p><strong>Price:</strong> $299,200</p>
      <p><strong>Specs:</strong> 3 Beds | 2.5 Baths | 1,419 sqft | Built 2024</p>
      <p>New construction with double vanity, tray ceilings, spacious owner's suite, and walk-in closet. Quiet Mustang Ridge location near schools and shopping.</p>
      <a href="https://www.zillow.com/homedetails/142-Pinto-Ln-SE-Fairmount-GA-30139/443999964_zpid/" target="_blank" class="button">Schedule a Viewing</a>
    </div>
  </div>

  <div class="listing" data-price="294200" data-beds="3" data-type="New Construction">
    <img src="https://photos.zillowstatic.com/fp/d9bb99cf407aaa50b1e0e26059906c80-uncropped_scaled_within_1344_1008.webp" alt="154 Pinto Ln SE">
    <div class="info">
      <h2>154 Pinto Ln SE, Fairmount, GA 30139</h2>
      <p><strong>MLS #:</strong> 401187</p>
      <p><strong>Price:</strong> $294,200</p>
      <p><strong>Specs:</strong> 3 Beds | 2.5 Baths | 1,419 sqft | Built 2024</p>
      <p>Stylish and energy-efficient new build in Mustang Ridge. Open layout, updated flooring, modern kitchen, attached garage, and spacious owner's suite.</p>
      <a href="https://www.zillow.com/homedetails/154-Pinto-Ln-Fairmount-GA-30139/452102812_zpid/" target="_blank" class="button">Schedule a Viewing</a>
    </div>
  </div>

  <div class="listing" data-price="294200" data-beds="3" data-type="New Construction">
    <img src="https://photos.zillowstatic.com/fp/d9bb99cf407aaa50b1e0e26059906c80-uncropped_scaled_within_1344_1008.webp" alt="154 Pinto Ln SE">
    <div class="info">
      <h2>154 Pinto Ln SE, Fairmount, GA 30139</h2>
      <p><strong>MLS #:</strong> 401187</p>
      <p><strong>Price:</strong> $294,200</p>
      <p><strong>Specs:</strong> 3 Beds | 2.5 Baths | 1,419 sqft | Built 2024</p>
      <p>Stylish and energy-efficient new build in Mustang Ridge. Open layout, updated flooring, modern kitchen, attached garage, and spacious owner's suite.</p>
      <a href="https://www.zillow.com/homedetails/154-Pinto-Ln-Fairmount-GA-30139/452102812_zpid/" target="_blank" class="button">Schedule a Viewing</a>
    </div>
  </div>

  <div class="listing" data-price="364900" data-beds="3" data-type="New Construction">
    <img src="https://photos.zillowstatic.com/fp/40a69a6684d60230e29aafa28c56f4e2-uncropped_scaled_within_1344_1008.webp" alt="240 Rivers Edge Dr">
    <div class="info">
      <h2>240 Rivers Edge Dr, Chatsworth, GA 30705</h2>
      <p><strong>MLS #:</strong> 412903</p>
      <p><strong>Price:</strong> $364,900</p>
      <p><strong>Specs:</strong> 3 Beds | 2.5 Baths | 1,699 sqft | Built 2024</p>
      <p>Gated, no-HOA community with private lake access. Craftsman-style ranch on a private 1+ acre wooded lot with granite kitchen, covered porch, and oversized garage.</p>
      <a href="https://www.zillow.com/homedetails/240-Rivers-Edge-Dr-Chatsworth-GA-30705/2057329026_zpid/" target="_blank" class="button">Schedule a Viewing</a>
    </div>
  </div>

  <div class="listing" data-price="449900" data-beds="3" data-type="House">
    <img src="https://photos.zillowstatic.com/fp/be5a7a302ec9b48292c450a5d39c480f-cc_ft_1536.webp" alt="3065 Kings Dr NW">
    <div class="info">
      <h2>3065 Kings Dr NW, Kennesaw, GA 30144</h2>
      <p><strong>MLS #:</strong> 407206</p>
      <p><strong>Price:</strong> $449,900</p>
      <p><strong>Specs:</strong> 3 Beds | 2 Baths | 1,840 sqft | Built 1999</p>
      <p>Four-sided brick ranch less than a mile from KSU. No HOA. Features open floor plan, double vanity primary bath, spacious kitchen, and large garage. Perfect for investors or homeowners alike.</p>
      <a href="https://www.zillow.com/homedetails/3065-Kings-Dr-NW-Kennesaw-GA-30144/35815785_zpid/" target="_blank" class="button">Schedule a Viewing</a>
    </div>
  </div>

  <div class="listing" data-price="169000" data-beds="0" data-type="Land">
    <img src="https://photos.zillowstatic.com/fp/fcb894fda9f7aba71359617667a8de9d-cc_ft_1536.webp" alt="820 Falcon Heights #3079">
    <div class="info">
      <h2>820 Falcon Heights #3079, Big Canoe, GA 30143</h2>
      <p><strong>MLS #:</strong> 400003</p>
      <p><strong>Price:</strong> $169,000</p>
      <p><strong>Specs:</strong> 0.78 acres | Vacant Land</p>
      <p>Private, wooded lot in the gated mountain resort of Big Canoe. Access to golf, lakes, hiking trails, fitness center, clubhouse, and more. Utilities available. Build your dream retreat in the trees.</p>
      <a href="https://www.zillow.com/homedetails/820-Falcon-Hts-Jasper-GA-30143/97977230_zpid/" target="_blank" class="button">Schedule a Viewing</a>
    </div>
  </div>

  <div class="listing" data-price="349500" data-beds="2" data-type="New Construction">
    <img src="https://photos.zillowstatic.com/fp/d794739b9eb03a24cc768e733b462b56-cc_ft_1536.webp" alt="727 Copper Trace Way">
    <div class="info">
      <h2>727 Copper Trace Way, Woodstock, GA 30189</h2>
      <p><strong>MLS #:</strong> 404716</p>
      <p><strong>Price:</strong> $349,500</p>
      <p><strong>Specs:</strong> 2 Beds | 2.5 Baths | 2,175 sqft | Built 2024</p>
      <p>Modern craftsman design on over ½ acre. No HOA. Open layout, custom finishes, fireplace, and large kitchen. Walkable to Etowah High and minutes from Downtown Woodstock.</p>
      <a href="https://www.zillow.com/homedetails/727-Copper-Trace-Way-Woodstock-GA-30189/349587117_zpid/" target="_blank" class="button">Schedule a Viewing</a>
    </div>
  </div>

  <!-- Repeat the listing block above for your remaining 11 listings -->
  <!-- Make sure to update data-price, data-beds, and data-type accordingly -->

  <script>
    document.getElementById('filterBtn').addEventListener('click', function() {
      const price = document.getElementById('priceFilter').value;
      const beds = document.getElementById('bedFilter').value;
      const type = document.getElementById('typeFilter').value;
      const query = document.getElementById('searchInput').value.toLowerCase();
      document.querySelectorAll('.listing').forEach(listing => {
        const priceVal = parseInt(listing.dataset.price);
        const bedsVal = parseInt(listing.dataset.beds);
        const typeVal = listing.dataset.type;
        const textContent = listing.innerText.toLowerCase();
        let visible = true;
        if (price === '$100k - $300k' && priceVal > 300000) visible = false;
        if (price === '$300k - $500k' && (priceVal < 300000 || priceVal > 500000)) visible = false;
        if (price === '$500k+' && priceVal < 500000) visible = false;
        if (beds !== 'Bedrooms' && bedsVal < parseInt(beds)) visible = false;
        if (type !== 'Property Type' && type !== typeVal) visible = false;
        if (query && !textContent.includes(query)) visible = false;
        listing.style.display = visible ? 'flex' : 'none';
      });
    });
  </script>

</body>

</html>
