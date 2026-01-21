<h1 class="text-2xl text-white font-bold mb-2">AUTO-SCRAPER + SPATIAL DB</h1>
<div class="text-gray-500 text-xs mb-4 border-b border-gray-700 pb-2">DATE: 2024-2025 // LOC: SHANGHAI</div>

<div class="flex gap-2 mb-8">
<span class="px-2 py-1 bg-yellow-900 text-yellow-200 border border-yellow-700 rounded text-xs">SELENIUM</span>
<span class="px-2 py-1 bg-blue-900 text-blue-200 border border-blue-700 rounded text-xs">POSTGIS</span>
<span class="px-2 py-1 bg-green-900 text-green-200 border border-green-700 rounded text-xs">DOCKER</span>
<span class="px-2 py-1 bg-purple-900 text-purple-200 border border-purple-700 rounded text-xs">FLASK</span>
</div>

<div class="mb-8">
<a href="https://github.com/haoruizhou/SpatialDB" target="_blank" class="px-3 py-2 bg-amber-900/50 hover:bg-amber-800 text-amber-200 rounded border border-amber-700 text-sm transition">VIEW REPOSITORY &rarr;</a>
</div>

<h3>// SYSTEM ARCHITECTURE</h3>
<div class="grid grid-cols-2 gap-3 font-mono text-xs mb-6">
<div class="bg-gray-900 p-4 border border-gray-700 rounded cursor-pointer hover:border-amber-500 transition group select-none" onclick="toggleStatus(this)">
<div class="text-gray-500 mb-2 text-[10px] tracking-wider">WEB_SCRAPER</div>
<div class="status-indicator text-green-500 font-bold flex items-center gap-2">
<span class="w-2 h-2 rounded-full bg-green-500 shadow-[0_0_5px_rgba(34,197,94,0.8)]"></span> ACTIVE
</div>
</div>
<div class="bg-gray-900 p-4 border border-gray-700 rounded cursor-pointer hover:border-amber-500 transition group select-none" onclick="toggleStatus(this)">
<div class="text-gray-500 mb-2 text-[10px] tracking-wider">POSTGIS_DB</div>
<div class="status-indicator text-green-500 font-bold flex items-center gap-2">
<span class="w-2 h-2 rounded-full bg-green-500 shadow-[0_0_5px_rgba(34,197,94,0.8)]"></span> ACTIVE
</div>
</div>
<div class="bg-gray-900 p-4 border border-gray-700 rounded cursor-pointer hover:border-amber-500 transition group select-none" onclick="toggleStatus(this)">
<div class="text-gray-500 mb-2 text-[10px] tracking-wider">GEOCODER_WORKER</div>
<div class="status-indicator text-green-500 font-bold flex items-center gap-2">
<span class="w-2 h-2 rounded-full bg-green-500 shadow-[0_0_5px_rgba(34,197,94,0.8)]"></span> ACTIVE
</div>
</div>
<div class="bg-gray-900 p-4 border border-gray-700 rounded cursor-pointer hover:border-amber-500 transition group select-none" onclick="toggleStatus(this)">
<div class="text-gray-500 mb-2 text-[10px] tracking-wider">GEOSERVER_WMS</div>
<div class="status-indicator text-green-500 font-bold flex items-center gap-2">
<span class="w-2 h-2 rounded-full bg-green-500 shadow-[0_0_5px_rgba(34,197,94,0.8)]"></span> ACTIVE
</div>
</div>
</div>

<h3>// PROJECT OVERVIEW</h3>
<p>A comprehensive spatial database solution designed to simplify data collection, comparison, and mapping during market research and analysis. Integrates automated web scraping with geospatial tools in a unified Docker-based workflow.</p>

<h3>// TECHNICAL HIGHLIGHTS</h3>
<p><strong>Dual Coordinate System Support:</strong> Automatically manages both global WGS-84 (EPSG:4326) and national standard GCJ-02 (EPSG:4490) coordinate systems with automated transformation algorithms.</p>

<p><strong>Automated Geocoding:</strong> Flask-based background service converts addresses to coordinates using the Amap API, running automatically within 10 seconds of new data entry.</p>

<p><strong>Spatial Analysis:</strong> PostGIS-powered queries enable complex geospatial operations like proximity searches, distance calculations, and spatial relationships.</p>

<h3>// MICROSERVICES ARCHITECTURE</h3>
<p>The system is built on Docker Compose orchestrating multiple services:</p>
<ul>
<li><strong>PostGIS Database:</strong> Spatial data storage with dual coordinate system support</li>
<li><strong>Flask API:</strong> Geocoding service and backend API</li>
<li><strong>GeoServer:</strong> WMS/WFS services for geospatial data sharing</li>
<li><strong>MapStore:</strong> Web GIS client for creating and sharing maps</li>
<li><strong>PgAdmin:</strong> Database management interface</li>
</ul>

<h3>// ENGINEERING</h3>
<p>I engineered a complete geospatial data pipeline that combines automated web scraping with sophisticated spatial database capabilities. The scraper component (unreleased) collects market data, while the spatial database handles geocoding, coordinate transformation, and complex spatial queries for market research analysis.</p>