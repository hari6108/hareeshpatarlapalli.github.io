# hareeshpatarlapalli.github.io
import React from "react";
import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";
import { Github, Linkedin } from "lucide-react";

export default function Portfolio() {
  return (
    <main className="p-8 max-w-4xl mx-auto">
      <section className="mb-10 text-center">
        <h1 className="text-4xl font-bold mb-2">Hareesh Patarlapalli</h1>
        <p className="text-lg text-gray-600 mb-4">
          Geospatial Analyst | GIS & Remote Sensing | Civil Engineering
        </p>
        <div className="flex justify-center gap-4">
          <a
            href="https://www.linkedin.com/in/hareesh-patarlapalli-3833a3358"
            target="_blank"
            rel="noopener noreferrer"
          >
            <Button variant="outline">
              <Linkedin className="mr-2" /> LinkedIn
            </Button>
          </a>
          <a
            href="https://github.com/hari6108/mywork.git"
            target="_blank"
            rel="noopener noreferrer"
          >
            <Button variant="outline">
              <Github className="mr-2" /> GitHub
            </Button>
          </a>
        </div>
      </section>

      <section className="mb-10">
        <h2 className="text-2xl font-semibold mb-4">Projects</h2>
        <div className="grid gap-4">
          <Card>
            <CardContent className="p-4">
              <h3 className="text-xl font-medium">Air Quality Analysis – Delhi</h3>
              <p className="text-gray-600">
                Analyzed NO₂ & PM2.5 using satellite imagery; created hotspot maps in ArcGIS
                for targeted mitigation. Identified 12+ zones with over 30% increase in NO₂.
              </p>
            </CardContent>
          </Card>
          <Card>
            <CardContent className="p-4">
              <h3 className="text-xl font-medium">Urban Water Network Design</h3>
              <p className="text-gray-600">
                Designed GIS-based water distribution using WaterGEMS; optimized pressure loss
                by 25% and visualized hydraulic parameters in QGIS.
              </p>
            </CardContent>
          </Card>
        </div>
      </section>

      <section className="mb-10">
        <h2 className="text-2xl font-semibold mb-4">Experience</h2>
        <ul className="list-disc list-inside text-gray-700 space-y-2">
          <li>
            <strong>IISc Research Intern:</strong> GIS in sustainability & materials research
          </li>
          <li>
            <strong>The Standard Consultants:</strong> DGPS surveying & CAD-based planning
          </li>
          <li>
            <strong>VSR Infra Projects:</strong> Spatial drafting for residential layouts
          </li>
        </ul>
      </section>

      <section>
        <h2 className="text-2xl font-semibold mb-4">Skills & Tools</h2>
        <p className="text-gray-700">
          ArcGIS, QGIS, Google Earth Engine, Python (GeoPandas, Rasterio), WaterGEMS,
          AutoCAD, DGPS Surveying, Power BI
        </p>
      </section>
    </main>
  );
}
